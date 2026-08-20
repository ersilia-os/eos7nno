# CYP2D6 metabolism

Predicts both inhibition of cytochrome P450 2D6 and whether a molecule serves as its substrate. CYP2D6 is among the most strongly polymorphic drug-metabolising enzymes, and compounds cleared predominantly through it show pronounced inter-individual variability. The models come from an NCATS study that built QSAR predictors for catalysis and inhibition across CYP2C9, 2D6 and 3A4, aiming to flag isoform reliance early rather than after microsomal screening. Predictions describe enzyme interaction, not overall clearance.

This model was incorporated on 2023-07-06.Last packaged on 2025-10-17.

## Information
### Identifiers
- **Ersilia Identifier:** `eos7nno`
- **Slug:** `ncats-cyp2d6`

### Domain
- **Task:** `Annotation`
- **Subtask:** `Activity prediction`
- **Biomedical Area:** `ADMET`
- **Target Organism:** `Homo sapiens`
- **Tags:** `CYP450`, `ADME`, `Metabolism`

### Input
- **Input:** `Compound`
- **Input Dimension:** `1`

### Output
- **Output Dimension:** `2`
- **Output Consistency:** `Fixed`
- **Interpretation:** Probability of inhibiting CYP2D6 and probability of being a substrate of the enzyme.

Below are the **Output Columns** of the model:
| Name | Type | Direction | Description |
|------|------|-----------|-------------|
| cyp2d6_inhib | float | high | Probability of inhibition of the CYP2D6 |
| cyp2d6_subs | float | high | Probability of being metabolized by CYP2D6 |


### Source and Deployment
- **Source:** `Local`
- **Source Type:** `External`
- **DockerHub**: [https://hub.docker.com/r/ersiliaos/eos7nno](https://hub.docker.com/r/ersiliaos/eos7nno)
- **Docker Architecture:** `AMD64`, `ARM64`
- **S3 Storage**: [https://ersilia-models-zipped.s3.eu-central-1.amazonaws.com/eos7nno.zip](https://ersilia-models-zipped.s3.eu-central-1.amazonaws.com/eos7nno.zip)

### Resource Consumption
- **Model Size (Mb):** `2082`
- **Environment Size (Mb):** `2460`
- **Image Size (Mb):** `6300.95`

**Computational Performance (seconds):**
- 10 inputs: `33.65`
- 100 inputs: `23.92`
- 10000 inputs: `364.05`

### References
- **Source Code**: [https://github.com/ncats/ncats-adme](https://github.com/ncats/ncats-adme)
- **Publication**: [https://doi.org/10.1124/dmd.120.000320](https://doi.org/10.1124/dmd.120.000320)
- **Publication Type:** `Peer reviewed`
- **Publication Year:** `2021`
- **Ersilia Contributor:** [ZakiaYahya](https://github.com/ZakiaYahya)

### License
This package is licensed under a [GPL-3.0](https://github.com/ersilia-os/ersilia/blob/master/LICENSE) license. The model contained within this package is licensed under a [None](LICENSE) license.

**Notice**: Ersilia grants access to models _as is_, directly from the original authors, please refer to the original code repository and/or publication if you use the model in your research.


## Use
To use this model locally, you need to have the [Ersilia CLI](https://github.com/ersilia-os/ersilia) installed.
The model can be **fetched** using the following command:
```bash
# fetch model from the Ersilia Model Hub
ersilia fetch eos7nno
```
Then, you can **serve**, **run** and **close** the model as follows:
```bash
# serve the model
ersilia serve eos7nno
# generate an example file
ersilia example -n 3 -f my_input.csv
# run the model
ersilia run -i my_input.csv -o my_output.csv
# close the model
ersilia close
```

## About Ersilia
The [Ersilia Open Source Initiative](https://ersilia.io) is a tech non-profit organization fueling sustainable research in the Global South.
Please [cite](https://github.com/ersilia-os/ersilia/blob/master/CITATION.cff) the Ersilia Model Hub if you've found this model to be useful. Always [let us know](https://github.com/ersilia-os/ersilia/issues) if you experience any issues while trying to run it.
If you want to contribute to our mission, consider [donating](https://www.ersilia.io/donate) to Ersilia!
