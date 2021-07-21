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
