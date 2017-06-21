# experimenting with a recurrent neural network package

## what I was trying to do
- I was curious to figure out if I could train the computer to write an Indiana Jones script. To do this, you put together a file to show the computer what such a script looks like. This is the 'training' file, or the input.txt
- I googled until I found the scripts. I used Raiders, Temple of Doom, and Last Crusade
- reading the documentation for [char-rnn](https://github.com/karpathy/char-rnn) I realized that was too small, so I added Goonies and the Brendan Frasier Mummy. 

## what I did
- I followed the instructions at https://github.com/karpathy/char-rnn to download and install the char-rnn package
- the last instruction, about sourcing, I had to re-run when I logged back into dhbox
- today's history.txt file is [june21-todays-history-file.txt](june21-todays-history-file.txt)

## things that were hard
- getting the data. I went to gist.github.com and made a file, [input.txt](https://gist.github.com/shawngraham/af1edaa5b40be09d643a4700bb2150af)
- I used curl to download it to the data folder, but had to find the 'raw' version, otherwise i just got the html that wraps the gist page. Raw version is behind the raw button on the page, [here](https://gist.githubusercontent.com/shawngraham/af1edaa5b40be09d643a4700bb2150af/raw/14c6a48715f20725256b9b2ccd13eeb3a3372fcd/input.txt]
- trained the rnn with this command: `th train.lua -data_dir data/input.txt -rnn_size 512 -num_layers 2 -dropout 0.5`
- came back the next day, when it finished running (which is today). Had to enter the source command again before dhbox remembered where torch was installed - i cd'd into the torch folder to do that
- 'sampled' the model - this runs the generate-a-new-script thing `th sample.lua cv/some_checkpoint.t7 -gpuid -1`
- had to ls the cv folder so I would know the file name for the last checkpoint. 
- this printed the result to the screen; to do it to a file I added the > filename thing: `th sample.lua cv/some_checkpoint.t7 -gpuid -1 > script.txt`

## thoughts on where to go next

this ends the example. You could link to annotations you made, things you've seen, work that this entry is in dialog with, and so on. 
