# NoCy transformer language model

A simple transformer language model based on bert and tuned with the norwegian (bokmål) NorNE dataset.

Due to its size, the not included but you can easily recreate it:
- Create the folders `assets` and `packages`
- Run `python -m spacy project run nocy_nb`


This project is the result of shamelessly duct-taping together the default Spacy suggested config for a norwegian transformer model, and a bastardized copy of Kenneth Enevoldsen's repo doing mostly the same thing to create a danish transformer model: https://github.com/KennethEnevoldsen/DaCy. Even the name was copied.