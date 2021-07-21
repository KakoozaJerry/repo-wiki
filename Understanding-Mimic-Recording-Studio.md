There is a silent buffer introduced at the beginning

https://github.com/MycroftAI/mimic-recording-studio/blob/e57b1ffd4083429fe1297a326a7092f42a110250/backend/app/audio.py#L16

Above they trim 300ms at both the start and at the end of the recording, this can be changed as you find best fit since sometimes it may cut off some spoken words