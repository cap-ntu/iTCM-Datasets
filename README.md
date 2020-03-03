# iTCM-Datasets

This research proposes to develop online thermal comfort models via a deep-learning approach and apply them to behavioral studies to drive “greener, smarter and healthier buildings” in the tropics (e.g., Singapore). Leveraging privacy-preserving data analytics over information acquired from smartphone crowdsourcing and in-situ wearables measurements, the project plans to develop and validate an integrative, economical and scalable thermal comfort management system.

## Metadata

Canonical URL: [https://researchdata.ntu.edu.sg](https://researchdata.ntu.edu.sg)

Title: Related data for: Heterogeneous Transfer Learning for Thermal Comfort Modeling

Related Publication: Weizheng Hu, Yong Luo, Zongqing Lu, and Yonggang Wen. 2019. Heterogeneous Transfer Learning for Thermal Comfort Modeling. In Proceedings of the 6th ACM International Conference on Systems for Energy-Efficient Buildings, Cities, and Transportation (BuildSys ’19). Association for Computing Machinery, New York, NY, USA, 61–70. doi: 10.1145/3360322.3360843

Grant Information: Building and Construction Authority (BCA) Singapore: NRF2015ENC-GBICRD001-012

Subject: Computer and Information Science; Medicine, Health and Life Sciences

Keywords: thermal comfort, heart rate, skin temperature, HVAC, air-conditioning, thermal sensation, predicted mean vote (PMV)

## Instruction

Those files with name `no_3_thermal` are used in Buildsys 2019 paper, the reason is:

> We notice that the total number of +3 (hot) votes is deficient. There are only 31 “hot” votes received from 14 participants in our datasets. Thus, we consider that these “hot” votes cannot correctly reflect most of the participants' hot sensations and decide to remove them from both iTCM datasets.

```
.
├── Datasets
│   ├── buildsys_19_dataset_4314.csv
│   ├── buildsys_19_dataset_person1_346.csv
│   ├── buildsys_19_dataset_person2_385.csv
│   └── buildsys_19_dataset_person3_345.csv

// Datasets without "hot" (+3) votes (Used in Buildsys 2019 paper)
│   ├── buildsys_19_dataset_4293_no_3_thermal_index.csv ()
│   ├── buildsys_19_dataset_person1_345_no_3_thermal_index.csv
│   ├── buildsys_19_dataset_person2_380_no_3_thermal_index.csv
│   ├── buildsys_19_dataset_person3_341_no_3_thermal_index.csv
├── Documents
│   ├── 1) readme.txt
│   ├── 2) Experiment Introduction.docx
│   ├── 3) Dataset Features & Codes.docx
│   └── 4) Dataset v1 Information.docx
└── README.md

2 directories, 13 files
```

## Sample Data

You may find the explaination of each field in `Dataset v1 Information.docx`.

| id | user\_uuid                               | hour | age | weight | height | gender | at          | rh          | met          | cl    | hr | st | ati\(\-3\-2\) | ati\(0\-5\) |
|----|------------------------------------------|------|-----|--------|--------|--------|-------------|-------------|--------------|-------|----|----|---------------|-------------|
| 1  | 1b5d595c\-1bb9\-4f20\-a78a\-217958689877 | 21   | 19  | 74     | 170    | 1      | 25\.33358   | 55\.03636   | 1\.192368839 | 0\.54 | 74 | 31 | 0             | 3           |
| 2  | 1b5d595c\-1bb9\-4f20\-a78a\-217958689877 | 21   | 19  | 74     | 170    | 1      | 25\.2573745 | 58\.3366765 | 1\.169438669 | 0\.54 | 73 | 32 | \-1           | 2           |
| 3  | 1b5d595c\-1bb9\-4f20\-a78a\-217958689877 | 21   | 19  | 74     | 170    | 1      | 25\.311282  | 59\.00144   | 1\.207590569 | 0\.54 | 92 | 32 | 0             | 3           |
| 4  | 1b5d595c\-1bb9\-4f20\-a78a\-217958689877 | 22   | 19  | 74     | 170    | 1      | 25\.334916  | 58\.009603  | 1\.113437381 | 0\.54 | 72 | 32 | \-1           | 2           |
| 5  | 1b5d595c\-1bb9\-4f20\-a78a\-217958689877 | 22   | 19  | 74     | 170    | 1      | 25\.333581  | 56\.980052  | 1\.184626185 | 0\.54 | 77 | 32 | \-1           | 2           |
| 6  | 1b5d595c\-1bb9\-4f20\-a78a\-217958689877 | 22   | 19  | 74     | 170    | 1      | 25\.1385505 | 55\.5704215 | 1\.146804373 | 0\.54 | 77 | 33 | 1             | 4           |
| 7  | 1b5d595c\-1bb9\-4f20\-a78a\-217958689877 | 22   | 19  | 74     | 170    | 1      | 25\.1385505 | 55\.5704215 | 1\.136650669 | 0\.54 | 79 | 33 | 0             | 3           |
| 8  | 1b5d595c\-1bb9\-4f20\-a78a\-217958689877 | 22   | 19  | 74     | 170    | 1      | 25\.1918955 | 54\.5402515 | 1\.184330398 | 0\.54 | 79 | 33 | 1             | 4           |
| 9  | 1b5d595c\-1bb9\-4f20\-a78a\-217958689877 | 22   | 19  | 74     | 170    | 1      | 25\.261325  | 53\.424551  | 1\.234368697 | 0\.54 | 83 | 32 | 1             | 4           |
| 10 | 1b5d595c\-1bb9\-4f20\-a78a\-217958689877 | 23   | 19  | 74     | 170    | 1      | 25\.218705  | 53\.0346485 | 1\.174277726 | 0\.54 | 80 | 32 | 0             | 3           |

## Scope of Dataset

| Dataset                | Size \(with hot votes\)                   | Air Temperature Range | Relative Humidity Range |
|------------------------|-------------------------------------------|-----------------------|-------------------------|
| iTCM generic dataset   | 4293 \(4314\)                             | 19\.6°C \- 30\.6°C    | 37\.3% \- 83\.6%        |
| iTCM personal datasets | 345 \(346\) \+ 380 \(385\) \+ 341 \(345\) | 19\.6°C \- 29\.9°C    | 42\.4% \- 75\.5%        |


## License

<a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" /></a>

This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/">Creative Commons Attribution-NonCommercial 4.0 International License</a>.