# ErrorIST

**ErrorIST** is a framework dedicated to the task of adding fine-grained error types to text, and, as much as possible, to automatically evaluate an editor's proficiency, which is usually a manual and expensive task


**ErrorIST** implements common error types, identified in frameworks such as the Multidimensional Quality Metric (MQM), and in taxonomies dedicated to translation errors such as the errors presented in [Costa, et. al. 2015](https://link.springer.com/article/10.1007/s10590-015-9169-0).

The following table summarizes the taxonomy of errors supported by **ErrorIST**:

- Punctuation (omission and addition)(ex: _I found **,** the clowns, Bob, and Clyde._);
- Capitalisation (ex: _**i** think my poor Slipper got dirty!_);
- Spelling (ex: _I have **three** friends._);
- Omission (content or function words) (ex: _His hat was []_);
- Addition (content or function words) (ex: _He bought a **already** hat._).
- Misselection
  - Word-class (ex: _The **cutely** bird is on the branch._);
  - Verbs (tense, person or both) (ex: _He had **buy** a suit-case._);
  - Agreement (gender, number or both; or person) (ex: _**Os lobo** fugiu._/_The Wolf run away_. In Portuguese, _Os_ is plural and _lobo_ singular.);
  - Contraction (ex: _Ela senta-se **em a** cadeira._/_She seats in the chair_. In Portuguese, _em_ + _a_ = _na_.).
- Misordering (ex: _I **beautiful** like the [] color of your eyes._).
- "Confusion of senses": when a word was translated into one of its possible meanings, but, in the given context, not the correct one.

## ErrorIST Architecture:

**ErrorIST** is  composed  of  three  modules:   **Error Generator**,  **Tracer**,  and **Evaluator**:
![errorist (1)](https://user-images.githubusercontent.com/17256847/122262890-c85ba980-cecd-11eb-8a16-bceffbab908e.jpg)

**Error Generator** generates the errors, **Tracer** analyses how the generated errors were corrected and **Evaluator** grades the modifications detected by **Tracer**; if it is not possible to automatically evaluate an error, a manual evaluation is requested.

## CODE 2.0
A second version of the code can be [downloaded here](https://drive.google.com/file/d/1xDX6o9IEKuV0ubjJwdtshYkOYBxUkKDl/view?usp=sharing)

## Bibliography

Two thesis contributed to the building of ErrorIST. They were developed by Tiago  Santos and Raquel Cristovão, and can be found [here](  https://fenix.tecnico.ulisboa.pt/departamentos/dei/dissertacao/565303595500952) and [here](https://fenix.tecnico.ulisboa.pt/downloadFile/281870113704582/76513%20-raquel%20-%20cristovao.pdf).
