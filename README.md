# GoPro Tests

## In one sentence

This repository exists to document GoPro camera footage that can be used for software tests.

## Why we built this

We build software that processes GoPro video and image files. To test this software we use a library of GoPro video and image content. This repository exist to document and share the test cases we use, should they be useful to anyone else.

## Download test cases

* Library of test cases: https://docs.google.com/spreadsheets/d/1CqShexm4B-PdvBT-MG5WU0706FTftE1PktYAYyF3peA/edit?usp=sharing
* Actual test case files: https://drive.google.com/drive/folders/10hiCdNWuk7OPdVAQ3LzYc94RqoJX1-cN?usp=sharing

## Cameras currently covered

* [Fusion](/fusion)
* [MAX](/max)
* [HERO 10](/hero10)

## Valid vs Invalid test cases

Typically you will be interested in the Valid test cases (`VALID TESTS`tab). These are unmodified outputs from GoPro cameras.

The `INVALID TESTS` tab contains test cases that should fail in our software, however, do not necessarily mean the file is corrupt. You can ascertain why it is an invalid test case for our purposes in the corresponding "Reason bad" column.

## License

* Code: [Apache 2.0](/LICENSE).
* Images: [CC BY-SA 4.0](/LICENSE-IMAGES).