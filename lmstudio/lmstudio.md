### Lm Studio

Lm Studio is a free and open-source application to run locallly downloaded large language models. It runs on Windows, Mac and Linux machines, and also comes with a cli tool to run
models in a headless environment.

I have installed Lm Studio on a machine with 16gb of ddr4 memory and a GTX 980ti graphics card. Despite this hardware being relatively old and rather inadequate to handle most AI 
models well, I was able to come accross a model that did run smoothly and still have enough parameters to complete most tasks well.

That model turned out to be Gemma 4 with 4B parameters, which also came with Vision, Tool use and reasoning capabilities. This model was able to fit primarily on the VRAM of my GPU
6GB, while only using a portion of my system memory.

However, by default I did not have any way to directly access web information that was not already in the parameters of the model. Luckily Lm studio allows for additional support to be
added through their plugins system. I found the duckduckgo and visit-website plugins from danielsig, and installed them using the "lms get danielsig/duckduckgo" and "lms get
danielsig/visit-website" commands respectively.

However I wanted to be able to access this model on other devices (primarily my laptop), but luckily there was already an inbuilt way to do that. Lm link allows for two instances of 
Lm studio to be connected together (provided they are both signed into the same account), on the same local network. Now I am able to access all the capabilities of the AI model running
on my PC while having the flexibility to get it's output anywhere throughout my house. Furthermore I am also able to connect remotely to my AI model from anywhere, as both my laptop and
PC are connected to Tailscale.

I have found great use out of Lm Studio and will continue to use it as more models come out, that are hopefully even more effecient, and the hardware I am able to run them on also
improves.

13.4.26 - 04:30 PM AEST
