# CYP2D6 Metabolism

Analysis of metabolic stability, determining the inhibition of CYP2D6 activity and whether the compounds are a substrate for the CYP2D6 enzyme. The data to build these models has been publicly available at PubChem (AID1645840, AID1645841, AID1645842) by ADME@NCATS

## Identifiers

* EOS model ID: `eos7nno`
* Slug: `ncats-cyp2d6`

## Characteristics

* Input: `Compound`
* Input Shape: `Single`
* Task: `Classification`
* Output: `Probability`
* Output Type: `Float`
* Output Shape: `List`
* Interpretation: Probability of inhibiting the enzyme and probability of being a ubstrate of the enzyme. Activity in both indicates the compound is a ligand of the enzyme.

## References

* [Publication](https://dmd.aspetjournals.org/content/49/9/822)
* [Source Code](https://github.com/ncats/ncats-adme)
* Ersilia contributor: [ZakiaYahya](https://github.com/ZakiaYahya)

## Ersilia model URLs
* [GitHub](https://github.com/ersilia-os/eos7nno)
* [AWS S3](https://ersilia-models-zipped.s3.eu-central-1.amazonaws.com/eos7nno.zip)
* [DockerHub](https://hub.docker.com/r/ersiliaos/eos7nno) (AMD64, ARM64)

## Citation

If you use this model, please cite the [original authors](https://dmd.aspetjournals.org/content/49/9/822) of the model and the [Ersilia Model Hub](https://github.com/ersilia-os/ersilia/blob/master/CITATION.cff).

## License

This package is licensed under a GPL-3.0 license. The model contained within this package is licensed under a None license.

Notice: Ersilia grants access to these models 'as is' provided by the original authors, please refer to the original code repository and/or publication if you use the model in your research.

## About Us

The [Ersilia Open Source Initiative](https://ersilia.io) is a Non Profit Organization ([1192266](https://register-of-charities.charitycommission.gov.uk/charity-search/-/charity-details/5170657/full-print)) with the mission is to equip labs, universities and clinics in LMIC with AI/ML tools for infectious disease research.

[Help us](https://www.ersilia.io/donate) achieve our mission!
