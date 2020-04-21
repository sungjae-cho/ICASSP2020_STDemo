# ICASSP Show and Tell Demonstration

Demo hompage link: [https://sungjae-cho.github.io/ICASSP2020_STDemo/](https://sungjae-cho.github.io/ICASSP2020_STDemo/)

## Learning to Transfer Multi-speaker Emotional Prosody to a Neutral Speaker

- **Conference:** [ICASSP 2020](https://2020.ieeeicassp.org/)
- **Session:** [Show and Tell](https://2020.ieeeicassp.org/program/show-tell/)
- **Presentation:** [slides](slides/ICASSP2020_ST_slides.pdf)
- **Presentation time:** Friday, 8 May, 11:45 – 13:45
- **Title:** **Learning to Transfer Multi-speaker Emotional Prosody to a Neutral Speaker**
- **Authors:** Authors Sungjae Cho, Sejik Park, Tae-Ho Kim, Soo-Young Lee
- **Abstract:** Most recent emotional speech synthesizers have been studied with a large training data. These systems require a sufficient number of audios to be recorded with respect to different emotions for each speaker. Acquiring emotional speech is more expensive than acquiring neutral speech because it requires professional acting ability to express natural emotional utterance in the voice recording environment. Thus, it would be economical, beneficial to transfer decent emotional prosody to neutral voice. We demonstrate our system can learn to speak the emotional speech of multiple speakers from their emotional audios, and transfer emotional prosody to the voice of a speaker who provides only neutral speech. Our system is a neural network architecture that synthesizes speech directly from text and emotion and speaker identifiers. This architecture is mainly composed of two components: modified Tacotron 2 and original WaveGlow. Tacotron 2 is a recurrent sequence-to-sequence network that maps character embeddings to mel-spectrograms; WaveGlow is a vocoder to synthesize time-domain waveforms from those spectrograms. The modified Tacotron 2 has been trained to synthesize speech from text depending on emotions and speakers by modification of injecting emotion and speaker encoding into the decoder part of Tacotron 2. This allows the system to learn to synthesize not only emotional speech of speakers with emotional audios but also that of a speaker without emotional audios. In this demo, audience can interactively enter any sentence to the speech synthesis system. Additionally, speech synthesis markup language (SSML) has been incorporated to easily control prosody of spoken input text. With the provided SSML, audience can manipulate emotion and speaker as well as three basic components: rate, volume, and pitch for fine-tuning. These three components are controllable at the character-level. The positions of characters spoken in the mel-spectrogram are estimated from which characters are highly attended to generate each mel-spectrogram.

In this demo, we are unable to provide an interactive environment that incorporates SSML to easily control prosody of input text. We aplogize for no provision of an interactive environment.

All of the below phrases are unseen by our TTS model during training.

### Demo 1: Multi-speaker emotional TTS

In the first demo, we are demonstrating multi-speaker emotional TTS. Through our system, you can synthesize 5 emotional voices across two female speakers: B and J. In the training data, we had neutral and emotional speech audios of the two speakers. This is a major difference with the second demo. I'm going to play 3 examples for each emotion-speaker pair. What we want you to pay attention to is how different given audios are across emotions and speakers. First, you will listen to a neural voice, and then an emotional voice will be presented.

To listen to audios, go to [https://sungjae-cho.github.io/ICASSP2020_STDemo/](https://sungjae-cho.github.io/ICASSP2020_STDemo/).

### Demo 2: Emotional TTS spoken by a neutral speaker

In the second demo, we are demonstrating emotional TTS spoken by a neutral speaker. Through our system, you can synthesize 5 emotional voices of a female speaker, L. In the training data, there were only neutral speech audios of the L speaker. Our system can generate emotional speech of the L speaker because emotional prosody has been transferred from the other two speakers' emotional prosody by jointly learning their emotional speech. Let’s listen to emotional voices of the L speaker.

To listen to audios, go to [https://sungjae-cho.github.io/ICASSP2020_STDemo/](https://sungjae-cho.github.io/ICASSP2020_STDemo/).
