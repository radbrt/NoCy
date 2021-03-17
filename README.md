# NoCy transformer language model

A simple transformer language model based on bert and tuned with the norwegian (bokmål) NorNE dataset.

Due to its size the model is not included but you can easily recreate it:
- Create the folders `packages` and `training`
- Run `python -m spacy project run nocy_nb`

## Great artists steal

This project is the result of shamelessly duct-taping together the default Spacy suggested config for a norwegian transformer model, and a bastardized copy of Kenneth Enevoldsen's repo doing mostly the same thing to create a danish transformer model: https://github.com/KennethEnevoldsen/DaCy. Even the name was copied.

Similarly, the conllu training data is lifted from https://github.com/ltgoslo/norne

## Metrics

|metric|score|
|---|---:|
token_acc|0.9986249455|
|tag_acc|0.9848847525|
|dep_uas|0.9403620269|
|dep_las|0.9250789688|
|ents_p|0.8749116608|
|ents_r|0.8951554591|
|ents_f|0.8849177984|
|sents_p|0.9803820341|
|sents_r|0.9793708097|
|sents_f|0.979876161|
