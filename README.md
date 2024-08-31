# pd-midiscratch
Pd abstraction for loading midi files and "scratching" through the notes (with dynamic duration)

## howto
* add folder to path
* create [midiscratch] object
* check help file

## known issues
* notes have to be passed by to get played. this is a problem for pieces starting at time:0. in that case, the input needs to go lower than 0
* there are some older abstractions for different approaches: handling note-off as note-on (and vice versa) on backwards play and the whole mechanism based on [text] and [text search] (which is too slow for midi files with more than 500k notes here)
* only notes on midi channel 1 are being parsed
