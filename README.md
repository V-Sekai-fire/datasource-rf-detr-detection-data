# datasource-rf-detr-detection-data

A clothing object-detection dataset, split into train and test Parquet files for fine-tuning a detector.

## What it is for

Each row holds one image, byte-identical to the source export, with its COCO-style category ids and bounding boxes. `categories.json` maps the category ids to names.

## Use

Read `train.parquet` and `test.parquet` with any Parquet reader. `gen_split.py` rebuilds them from the source project's COCO export.

## Licence

CC BY 4.0, for the data and for this repository's additions. [LICENSE.txt](LICENSE.txt) names the source project and its author.
