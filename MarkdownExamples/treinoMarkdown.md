~~Este é apenas um monte de palavras sem sentido no qual posso *praticar* **marcações de texto Markdown**~~

> "Fulano mencionou que Sicrano __*disse*__ algo para Beltrano"
> 
> "É mesmo?", disse Sicrano

``` c++
//To calculate each oscillator’s output in render():
//  Get the next sample of this oscillator
//•
//Task: fix additive-synth so that oscillators above the Nyquist rate are muted
//Problem: even with a limited number of harmonics, we might still have aliasing!
//‣

for(unsigned int n = 0; n < context->audioFrames; n++) {
 float out = 0;
 // Step through all the oscillators in the array
 for(unsigned int i = 0; i < gOscillators.size(); i++) {
 // Mix in the output of this oscillator
 out += gAmplitudes[i] * gOscillators[i].process();
 }
 // Scale global amplitude
 out *= amplitude;
 for(unsigned int channel = 0; channel < context->audioOutChannels; channel++) {
 // Write the sample to every audio output channel
 }
audioWrite(context, n, channel, out);
  // Write the output to the oscilloscope
 gScope.log(out);
 }
 
```

Android | iOS
--- | ---
App 1 | App 2
Environment A | Environment B
[download aqui](https://rifosi.com.br) | [UOL aqui](https://uol.com.br)
![](https://upload.wikimedia.org/wikipedia/commons/0/0a/Unofficial_Windows_logo_variant_-_2002%E2%80%932012_%28Multicolored%29.svg) | ![](ios.png)
# Cabeçalho1
## Cabeçalho2
###### Cabeçalho6
- primeiro elemento
- segundo elemento
+ [X] primeiro elemento
+ [ ] segundo elemento
* primeiro elemento
* segundo elemento
- primeiro elemento
- segundo elemento 

1. primeiro elemento
1. segundo elemento
   1. primeiro elemento
   1. segundo elemento

3. primeiro elemento
4.  segundo elemento
5.  primeiro elemento
6. segundo elemento 


