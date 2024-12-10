---
title: SemEval-2025 Task 1 - Training Data
---


### Subtask A - Static Images

#### English

English training data for Subtask A can be obtained here:

[Subtask A Training Data - English](https://drive.google.com/file/d/1D5zcLxejMpYMZUD63Ljd8LhV18MycJPY/view?usp=drive_link)

#### Portuguese

Portuguese training data for Subtask A can be obtained here:

[Subtask A Training Data - Portuguese](https://drive.google.com/file/d/1wXikkvk5wMP14GNWjkqm662IHKZbzN-R/view?usp=drive_link)


### Subtask B - Sequences

English training data for Subtask B are now available:

[Subtask B Training Data - English](https://drive.google.com/file/d/1SL_1ARAyyWRCq3a0Fq8qhWj8EJwpPY4k/view?usp=sharing)




If you'd like to examine a smaller sample of the (English) training data, see the [Sample Data page](/data/sample/sample_data.md).


### Data Description

The training datasets contain the folllowing files:

## Subtask A

AdMIRe Subtask A Train.zip

English training data for Subtask A.

70 items.


	subtask_a_train.tsv
		Tab-separated dataset.

		Columns:
		**compound**		The potentially idiomatic noun compound to which the other data relates. This compound will appear (once) within **sentence**.
    **subset**			Indicates the data subset to which the item belongs. Values: {Train, Sample, Dev, Test}. Only {Train, Sample} will appear in this dataset; the latter indicates that the item was included in the smaller sample data provided on the website. All items in this dataset can be used for training purposes.    
    **sentence_type**	Indicates which sense of **compound** is used in **sentence**. Values: {idiomatic, literal}. This field will _not_ be included in dev and test data and should not be consumed by participating systems. It is provided here for information and analysis purposes, and as a possible target for system component training.
    **sentence**		Target sentence in which **compound** appears.
    **expected_order**	List of image names. This is the target output for the shared task which will be used for evaluation. This field will not be included in dev and test datasets.
    **image{n}_name**	Filename of the nth candidate image. This file is located in the subfolder which shares its name with **compound**, e.g. "green fingers/10027562830.png".
    **image{n}_caption**	Machine-generated descriptive caption of the nth candidate image. This is intended for participants who do not wish to perform image processing, but may be used to supplement the image files if desired. Note that the descriptions may not accurately reflect the intended content of the image, as they are the output of automatic captioning.	

Note: {n} for image name and caption ranges from 1 to 5 inclusive.
Image name and caption fields are ordered by the (randomised) image filename.

    Subfolders
		One subfolder for each target **compound**. Each subfolder contains 5 image files, corresponding to the entries in **image1_name** to **image5_name**.


AdMIRe Subtask A PT Train.zip

Brazilian Portuguese training data for Subtask A.

32 items.


	subtask_a_train.tsv
		Tab-separated dataset.

		Columns:
		**compound**		The potentially idiomatic noun compound to which the other data relates. This compound will appear (once) within **sentence**.
    **subset**			Indicates the data subset to which the item belongs. Values: {Train, Dev, Test}. Only {Train} will appear in this dataset. All items in this dataset can be used for training purposes. 
    **sentence_type**	Indicates which sense of **compound** is used in **sentence**. Values: {idiomatic, literal}. This field will _not_ be included in dev and test data and should not be consumed by participating systems. It is provided here for information and analysis purposes, and as a possible target for system component training.
    **sentence**		Target sentence in which **compound** appears.
    **expected_order**	List of image names. This is the target output for the shared task which will be used for evaluation. This field will not be included in dev and test datasets.
    **image{n}_name**	Filename of the nth candidate image. This file is located in the subfolder which shares its name with **compound**, e.g. "green fingers/10027562830.png".
    **image{n}_caption**	Machine-generated descriptive caption of the nth candidate image. This is intended for participants who do not wish to perform image processing, but may be used to supplement the image files if desired. Note that the descriptions may not accurately reflect the intended content of the image, as they are the output of automatic captioning.
    **image{n}_caption_pt**	Machine-generated descriptive caption of the nth candidate image in Portuguese. Note that this is generated independently of the English caption, not as a direct translation.

Note: {n} for image name and caption ranges from 1 to 5 inclusive.
Image name and caption fields are ordered by the (randomised) image filename.

    Subfolders
		One subfolder for each target **compound**. Each subfolder contains 5 image files, corresponding to the entries in **image1_name** to **image5_name**.


## Subtask B

AdMIRe Subtask B Train.zip

English training data for Subtask B.

20 items.

	subtask_b_train.tsv
		Tab-separated dataset.

		Columns:
		compound		The potentially idiomatic noun compound to which the other data relates.
		subset			Indicates the data subset to which the item belongs. Values: {Train, Sample, Dev, Test}. Only {Train, Sample} will appear in this dataset; the latter indicates that the item was included in the smaller sample data provided on the website. All items in this dataset can be used for training purposes.
		sentence_type	Indicates which sense of compound is represented by the image sequence to be completed. Values: {idiomatic, literal}. This is the secondary target output for the shared task and will be used for evaluation. This field will not be included in dev and test datasets.
		expected_item	Filename of the candidate image which completes the image sequence. This is the primary target output for Subtask B and will be used for evaluation. This field will not be included in dev and test datasets.
		sequence_caption1	Machine-generated descriptive caption of the first sequence image, s1.png. This is intended for participants who do not wish to perform image processing, but may be used to supplement the image files if desired. Note that the descriptions may not accurately reflect the intended content of the image, as they are the output of automatic captioning.	
		sequence_caption2	Machine-generated descriptive caption of the secondt sequence image s2.png.
		image{n}_name	Filename of the nth candidate image. This file is located in the subfolder which shares its name with compound, e.g. “guinea pig/39992220482.png”.
		image{n}_caption	Machine-generated descriptive caption of the nth candidate image. This is intended for participants who do not wish to perform image processing, but may be used to supplement the image files if desired. Note that the descriptions may not accurately reflect the intended content of the image, as they are the output of automatic captioning.	

Note: {n} for candidate image name and caption ranges from 1 to 4 inclusive.
Candidate image name and caption fields are ordered by the (randomised) image filename.

	Subfolders
		One subfolder for each target compound. Each subfolder contains 6 image files. s1.png and s2.png are the first and second sequence images, respectively. The other 4 image files are the candidates for completion of the sequence, and correspond to the entries in image1_name to image4_name.
