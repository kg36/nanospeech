# nanospeech
This project is about reducing the compute needs for Automatic Keyword Spotting (KWS). Think of Alexa running off classic tiny 8-bit Arduino Uno micro controller at 2KB RAM, 16MHz, 32KB flash.
Wikipedia defines Keyword spotting (KWS) as follows: "Keyword spotting is a problem that was historically first defined in the context of speech processing. In speech processing, keyword spotting deals with the identification of keywords in utterances."

In my knowledge, this is the community's first successful attempt at porting KWS to such a small footprint. Previous attempts have gone upto 32-bit M0 cortex, which is still 10X more powerful.
This work required tweaking the FFT 8-bit Radix-4 algo for windowing & spectrum, quantized MFCC feature extraction, a novel algorithm for voice activity detection and lastly a simplified form of Recurrent Neural Network for continuous detection. All running realtime on Arduino itself!

Update #1: a demo video
https://www.youtube.com/watch?v=QuIqwvaiINM

Full maths and code upload: ETA 11th Oct 2020
Stay tuned!
