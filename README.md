# text-mining-cwk

## Dataset
[DialogRE](https://huggingface.co/datasets/dataset-org/dialog_re)

## How to access and download the BERT Model

The link to the model can be downloaded here:
[Google Drive](https://drive.google.com/file/d/1FLREjoMlPnMOyY2_KLRiJzgoryU_jQyk/view?usp=drive_link)

The path to the model should be supplied at PATH_TO_MODEL under the 'Inferencing' section of the BERT.ipynb notebook. If you are running the notebook locally, the path shall suffice alone. Otherwise if you are running on Google Colab, it's recommended that you download the model to your personal Google Drive space, and mount the drive to access the model. You can uncomment the relevant google drive lines as indicated in the notebook.

## How to supply custom input data to the model

Entries input_dialog, input_x and input_y are supplied with suitable examples. input_dialog is a multi-line string consisting of a series of lines where the label of each line (i.e. the word before the colon) is Speaker 1, Speaker 2 etc. The supplied example is not taken from the dataset, so if it is too time-consuming to think up or search for dialog, the user may opt to experiment with the example. Alternatively, one can use LLM's such as ChatGPT with a prompt to generate dialog between Speaker 1 to n and supply the dialog as input. It is worth noting that order of x and y matters so think of the relation as x is (relation) to y. E.g. input_x being 'Rachel' and input_y being 'Ralph Lauren' would result in the relation org:employees_or_members, and swapping x and y would result in per:employee_or_member_of

## Use of Generative AI Tools

* Gemini - Was used inside of Google Colab for 'autocomplete', debug help, and explanation of modules/functions.
