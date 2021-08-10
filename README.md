# NoCy transformer language model

A simple transformer language model based on bert and tuned with the norwegian (bokmål) NorNE dataset.

The model is available on huggingface as `radbrt/nb_nocy_trf`, or you can recreate it from scratch by copying this project and:
- Create the folders `packages` and `training`
- Run `python -m spacy project run nocy_nb`

## Great artists steal

This project is the result of shamelessly duct-taping together the default Spacy suggested config for a norwegian transformer model, and a bastardized copy of Kenneth Enevoldsen's repo doing mostly the same thing to create a danish transformer model: https://github.com/KennethEnevoldsen/DaCy. Even the name was copied.

Similarly, the conllu training data is lifted from https://github.com/ltgoslo/norne, and the base model is `ltgoslo/norbert`


### Accuracy

| Type | Score |
| --- | --- |
| `TAG_ACC` | 98.80 |
| `POS_ACC` | 98.77 |
| `MORPH_ACC` | 98.01 |
| `DEP_UAS` | 94.34 |
| `DEP_LAS` | 92.52 |
| `SENTS_P` | 96.79 |
| `SENTS_R` | 97.68 |
| `SENTS_F` | 97.23 |
| `ENTS_F` | 90.46 |
| `ENTS_P` | 90.22 |
| `ENTS_R` | 90.70 |
| `TRANSFORMER_LOSS` | 1432675.77 |
| `TAGGER_LOSS` | 87954.00 |
| `MORPHOLOGIZER_LOSS` | 105773.67 |
| `PARSER_LOSS` | 1828631.17 |
| `NER_LOSS` | 81943.89 |
