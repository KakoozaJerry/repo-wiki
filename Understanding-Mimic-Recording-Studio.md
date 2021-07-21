## Cutting out silence at beginning and end
There is a silent buffer introduced at the beginning referenced in the link below

        `trim_buffer = 300  # buffer to prevent first sound getting cut` 

https://github.com/MycroftAI/mimic-recording-studio/blob/e57b1ffd4083429fe1297a326a7092f42a110250/backend/app/audio.py#L16

Above they trim 300ms at both the start and at the end of the recording, this can be changed as you find best fit since sometimes it may cut off some spoken words

## Sampling rate, and recording file format

By default mimic recording studio is recording sterio and with a sample rate of 44100Hz, this can be seen with the link below and the ac value represents 2 , this is not configurable by config files but you can change ac to 1 for mono files but good to stick with the default.

            ` 'ffmpeg -i {} -ab 160k -ac 2 -ar 44100 -vn {}.wav -y'.format( `

https://github.com/MycroftAI/mimic-recording-studio/blob/e57b1ffd4083429fe1297a326a7092f42a110250/backend/app/file_system.py#L45


## Corpus
This is found in the [prompts folder](https://github.com/MycroftAI/mimic-recording-studio/tree/master/backend/prompts)

Its in the form

    ` employment 10 `  
In a .csv file where we have the word followed by a tab, no white spaces then the number of characters 
To tell mimic recording studio to use the csv file I have put in the prompts, copy the name of the folder, shift to the [docker-compose.yml](https://github.com/MycroftAI/mimic-recording-studio/blob/master/docker-compose.yml) file in the root directory.
That means you need to have your docker environment readily setup.
Then substitute the environment - CORPUS value to default file

## Command line run
Shift to the directory where you cloned the repository and run

              ` docker-compose up `    

### Recording process
- The average speech rate will help you identify if you are too slow or too fast on recording after 20 recordings normally.
Start  a recording by hitting a space bar and the recording studio will automatically stop when you stop reading. 
Mimic uses the browser console to do the local storage of the recordings
> Removing the stored browser session data of recorded voice, 
- Move to inspect browser -> Application tab-> Local storage, There is a key value pair of the name and the token(UUID)
If you move back to the file explorer, you have more files than you had before. You can navigate to audio files and the UUID is the name of the folder of the spoken person as seen in the browser within this audio files folder.
- We also have a new directory db. Mimic recording studio uses sql to save the information.
- Open the db path in your database .
- Most relevant part is audiomodel. Each recording has a unique identifier.  There is an auto mapping between file name and text . 
- Think of more than 16 hours of speech recording for a good model.

