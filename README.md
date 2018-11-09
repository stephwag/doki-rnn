## The DDLC Mod that Keeps on Modding

This mod uses a recurrent neural network that continuously writes code for the game to execute. The result ranges from hilarious nonsense to downright terrifying nonsense.

![a](https://i.imgur.com/9yRtYCF.jpg)

### Temperature

Temperature is a setting to control the "creativity" of the neural net, anywhere between 0.0 to 2.0. The default is 1.0.

![a](https://i.imgur.com/Bh2Qv5s.png)

Generally speaking, since it is generating code, "creativity" may mean it will generate more buggy code (which may cause it to reload the script more often). However, it's there if you want to play with it anyways.

### How to Install

Install [Docker](https://docs.docker.com/install/#supported-platforms), then run `docker run -p 8081:8081 stephwag/doki`. The container must be running for the game to work. You can turn it off after you're done playing.

Copy `scripts.rpa` into the appropriate directory (and backup your original game files).