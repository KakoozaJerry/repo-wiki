## Luganda Text sources
[AI4Good](https://github.com/AI-Lab-Makerere/Data4Good) Luganda datasets from AI Lab at Makerere University
BBSTV [Twitter page](https://twitter.com/bbstvug) Scrap tweets
Radio Simba [Twitter Page](https://twitter.com/simbaradio) Scrap tweets
[GalaxyFM](https://www.galaxyfm.co.ug/luganda/) Website
[Preparing LJ Speech Datasets](https://github.com/eazhary/dctts2)
## TTS Engines
- [Ossian-Merlin](http://jrmeyer.github.io/tts/2017/09/15/Ossian-Merlin-demo.html)
- Coqui Engine [Newsletter](https://coqui.ai/)
- Mimic
- [Mozilla TTS ](https://stackoverflow.com/questions/66307611/how-do-i-get-started-training-a-custom-voice-model-with-mozilla-tts-on-ubuntu-20/66307612#66307612)
- colab notebook for [Voice Conversion with VITS:](https://colab.research.google.com/drive/1CO61pZizDj7en71NQG_aqqKdGaA_SaBf?usp=sharing)


- Y combinator [discussion on TTS](https://news.ycombinator.com/item?id=26790951) \

- https://github-wiki-see.page/m/coqui-ai/TTS/wiki/Implementing-a-New-Model-in-%F0%9F%90%B8TTS

- https://pythonrepo.com/repo/mozilla-TTS-python-natural-language-processing   Best resource for starter

[Blog post](https://erogol.com/gradual-training-with-tacotron-for-faster-convergence/) on how to train a Tacotron model faster for convergence

[Colab notebook](https://colab.research.google.com/drive/1OKnoOA69mnzr9kDY6lrnoitGo6Xk6ADl?usp=sharing) to train using Mozilla Tacotron 2 with DDC

[Page ](https://github-wiki-see.page/m/coqui-ai/TTS/wiki/Experimental-Released-Models) with various coqui TTS colab notebooks

https://github.com/tugstugi/pytorch-dc-tts

Tensor Board Upload

- https://tensorboard.dev/

## MOS - Mean Opinion Score
Calculating [MOS](https://www.microsoft.com/en-us/research/wp-content/uploads/2011/05/0002416.pdf)


## Audio Sources
[Edoboozi Lya Katikkiro](https://youtu.be/pOiupNeTibQ) ku BBS TV youtube

## Recording tools
- Mimic Recording Studio (It can show one the recording pace and also automatically treams beginning and ending silence)
- Audacity


##Helper script to convert Mimic recording studio data to LJSpeech format
[https://github.com/thorstenMueller/deep-learning-german-tts/blob/master/helperScripts/MRS2LJSpeech.py](https://github.com/thorstenMueller/deep-learning-german-tts/blob/master/helperScripts/MRS2LJSpeech.py)


## Luganda segment list, consonants on [phoible](https://phoible.org/inventories/view/770#tipa)
-[Vowels and Consonants from Irene's research](https://github.com/Nandutu/luganda_dataset)

| Inventory	| Language | Segments |Vowels | Consonants| Tones |
|-----------|----------|----------|-------|-----------|-------|
| luganda (AA 770)|	Ganda	|33	|10	|19	|4 |

##  Why - i think (open) voice is important
- Voice based human <-> machine interactions will come more
- Users expect decent quality on artificial voices (level set by Amazon/Google)
- Tech companies do not share voice models with community
- Level of trust and privacy is a concern on cloud based voices
- ???Talking devices??? might not be connected to the internet(for technical or security reasons)
- Companies might have money to buy ???voices??? but most open source communities won???t have this option
- For that i decided to contribute my voicewithout any licence restrictions (CC0)
- [Wikitounges](https://www.youtube.com/watch?v=AYgWSuv00pc)
- [Interesting translator](https://www.microsoft.com/en-us/translator/education/microsoft-teams-multilingual-meeting/)
- Even [google  cloud TTS](https://cloud.google.com/text-to-speech/docs/voices) has no Luganda localization for this
## Handling Demographic Biases in corpus
[Artie Bias Corpus](https://github.com/artie-inc/artie-bias-corpus): an audio corpus + code for detecting demographic bias 

## CV tool to split TEST,DEV, TRAIN sets
[CorporaCreator](https://github.com/mozilla/CorporaCreator)
> This ensures no single speaker is in more than one dataset of either dev, test or train sets even when they speak different sentences

## Research into existing similar Solutions
- [Mary TTS](http://mary.dfki.de/)
- [CMU Flite](http://www.festvox.org/flite/)
> topic modelling with [LDA for TTS and STT](https://www.aclweb.org/anthology/R15-1083.pdf
https://www.researchgate.net/publication/224382258_Latent_dirichlet_language_model_for_speech_recognition)
- [Create your own TTS with Coqui or mimic](https://www.youtube.com/watch?v=4YT8WZT_x48)

Why use LDA as opposed to neural networks
1. Its hard to understand why the neural network labelled an item wrong.
2. LDA can use as little datasets to get good results as opposed to neural networks that need large datasets.
[LDA models - Gensim](https://radimrehurek.com/gensim_3.8.3/models/ldamodel.html)

## Relevant Papers
#### Papers that used ChitChat Software an inhouse data collection tool
https://www.aclweb.org/anthology/L16-1317.pdf

https://storage.googleapis.com/pub-tools-public-publication-data/pdf/c5cf9f28ba2a9c0e50bc885bfad3bfbff3b4afbd.pdf

DDC - [Double Decoder Consistency](https://erogol.com/solving-attention-problems-of-tts-models-with-double-decoder-consistency/)

TTS (Model Architectures)[https://erogol.com/text-speech-deep-learning-architectures/]


1. [Open-Source Consumer-Grade Indic Text To Speech](https://www.cs.cmu.edu/~awb/papers/aup_ssw9_2016.pdf)
2. [Googles Tacotron paper](https://arxiv.org/pdf/1703.10135.pdf)
3. Text to speech synthesis for ethiopian semitic languages: [Issues and the way forward](https://ieeexplore.ieee.org/document/7331949/authors#authors) 
4. [Luganda Text-to-Speech Machine](https://arxiv.org/ftp/arxiv/papers/2005/2005.05447.pdf) uses 511 sentences from the bible to train with the MARYTTS by Irene Nandutu. 
5. [German Dataset](https://github.com/thorstenMueller/deep-learning-german-tts)
6. [HIU Audio German](https://github.com/iisys-hof/HUI-Audio-Corpus-German)

#### Flores Facebooks Low resource languages translator
[Github page](https://github.com/facebookresearch/flores)
[Google AI blog](https://ai.googleblog.com/search/label/TTS)


## Communities
[Mycroft AI](https://community.mycroft.ai/)
[Chat for Mycroft AI](https://chat.mycroft.ai)
[Coqui TTS engine](https://gitter.im/coqui-ai/TTS)
[Mozilla Discourse](https://discourse.mozilla.org/search?q=text%20to%20speech)
Mozilla's common voice deepspeech platform on [element](https://app.element.io/#/room/#common-voice:mozilla.org)

## Research done into Speech synthesis
https://youtu.be/qbPl0xoDnzQ
https://www.speech.kth.se/tts-demos/
speech that was not recorded with the purpose of being used in research (e.g. radio segments, public speeches, podcasts, archival recordings). Such data hold great worth in several regards but is typically challenging to work with.  ~ 
Per Fallgren 
[Edyson tool](https://github.com/perfall/Edyson)
Helpful [project PI](https://glottolog.org/resource/languoid/id/gand1255) for swedish thing Zofia Malisz and Per Fallgren
[Making Machines speak](https://www.youtube.com/watch?v=m-Uwb-Bg144&t=2303s)

> Develop a [vocal ID personna](https://vocalid.ai/about-us/)
We wouldn???t dream of fitting a little girl with the prosthetic limb of a grown man, why then was it okay to give her the same prosthetic voice as a grown man? - 
How to share your voice with [Local ID](https://vocalid.ai/voicebank/)


## Useful commands
> Working with `tar.gz files`
navigate to directory of the file and type in the commandline
`tar -xvf file_name.tar` 

> Other TTS or STT Platforms
[Ajala Studios](https://thespindle.org/project/speech-technologies-for-addressing-digital-access-in-africa/)
[Appen](https://appen.com/datasets/english-to-swahili-audio-recording-and-transcription/)
[Open Speech and Language Resources](https://openslr.org/)
[Lwazi Speech Corpus](https://sites.google.com/site/lwazispeechcorpus/)



> TTS Engines
[Great resource summarising all TTS](https://mycroft-ai.gitbook.io/docs/using-mycroft-ai/customizations/tts-engine#amazon-polly
)

[Mimic by microsoft](https://mycroft-ai.gitbook.io/docs/mycroft-technologies/mimic-overview)
[The mimic II platform](https://mycroft.ai/blog/mimic-2-is-live/)
The Mimic Recording Studio simplifies the collection of training data from individuals, each of which can be used to produce a distinct voice for Mimic.
[Corqui](https://coqui.ai/code)

[Baseline to compare already an existing Luganda STT for corqui](https://coqui.ai/luganda/itml/v0.1.0#model-details)

> Implement a Luganda TTS model on corqui
[example-synthesizing-speech-on-terminal-using-the-released-models](https://github.com/coqui-ai/TTS#example-synthesizing-speech-on-terminal-using-the-released-models)
[Implementing-a-New-Model](https://github.com/coqui-ai/TTS/wiki/Implementing-a-New-Model-in-%F0%9F%90%B8TTS)
Use the one stop [common utils shop](https://github.com/ftyers/commonvoice-utils) to pre process common voice data

`!CUDA_VISIBLE_DEVICES=0 python TTS/bin/train_tts.py --config_path config.json --restore_path pretrained.pth.tar --logdir "{toutdir}"`

## Running ngrok on colab to show tensorboards as you train
-https://gist.github.com/mrm8488/0a252982460134249a93cc92ef01deca 

## To prevent idle timeout in colab. 

Click inspect page or Press F12 OR CTRL + SHIFT + I 
Then paste what is below in your web console tab
```
function ClickConnect(){
console.log("Working");
document.querySelector("colab-toolbar-button#connect").click()
}
setInterval(ClickConnect,60000)
```


 