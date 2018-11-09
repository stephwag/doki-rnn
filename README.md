## The DDLC Mod that Keeps on Modding

This mod uses a recurrent neural network that continuously writes code for the game to execute. The result ranges from hilarious nonsense to downright terrifying nonsense.

<img width="50%" src="https://i.imgur.com/9yRtYCF.jpg"><img width="48%" src="https://i.imgur.com/fHj4Zmb.jpg">

### How to Install

Install [Docker](https://docs.docker.com/install/#supported-platforms), then run `docker run -p 8081:8081 stephwag/doki`. The container must be running for the game to work. You can turn it off after you're done playing.

Copy `scripts.rpa` into the appropriate directory (and backup your original game files).

### Playing the Game

#### Temperature

Temperature is a setting to control the "creativity" of the neural net, anywhere between 0.0 to 2.0. The default is 1.0.

![a](https://i.imgur.com/Bh2Qv5s.png)

Generally speaking, since it is generating code, "creativity" may mean it will generate more buggy code (which may cause it to reload the script more often). However, it's there if you want to play with it anyways.

#### Script Reloads and Exceptions

Since a neural net is programming the game, it will generate bad code every now and then. This cannot be helped.

If you see an exception giving you an option to either "ignore" it, choose that option. If that isn't available, click the "rollback" option (if available). If neither option is available, you may have to restart the game.

You may see the game go into "reload script" mode for a few seconds, then resume the game. This is because sometimes the generated code will cause something in memory to bug out, which also causes the Ren'Py parser to refuse loading new commands. Reloading script is basically a workaround for that.

You also may notice a very slight delay between each interaction. Generating dialogue takes a long time, and compared to other approaches I've tried, this seemed to be the least disruptive for gameplay. If I find a better way I'll update.