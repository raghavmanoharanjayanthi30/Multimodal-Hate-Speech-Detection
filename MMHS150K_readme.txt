--------------------
MMHS150K dataset
--------------------
Paper: "Exploring Hate Speech Detection in Multimodal Publications" 
Raul Gomez, Jaume Gibert, Lluis Gomez, Dimosthenis Karatzas
in WACV 2020
------
More info in : https://gombru.github.io/2019/10/09/MMHS/
------

----------------
Dataset contents
----------------

	img_resized/
		Images resized such that their shortest size is 500 pixels
		File name is image ID (same id as tweet ID)

	MMHS150K_GT.json
		Python dict with an entry per tweet, where key is the tweet ID and fields are:
			tweet_url 
			labels: array with 3 numeric labels [0-5] indicating the label by each one of the three AMT annotators
					0 - NotHate, 1 - Racist, 2 - Sexist, 3 - Homophobe, 4 - Religion, 5 - OtherHate
			img_url
			tweet_text
			labels_str: array with the 3 labels strings

	img_txt/
		Text extracted from the images using OCR.

	hatespeech_keywords.txt
		Contains the keyworkds that were used to gather the tweets.

	splits/train_ids.txt
	splits/val_ids.txt
	splits/test_ids.txt
		Contrain the tweet IDS used in the 3 splits



