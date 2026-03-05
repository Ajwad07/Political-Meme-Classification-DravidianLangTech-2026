# Political-Meme-Classification-DravidianLangTech-2026
# Gated Multimodal Fusion for Hierarchical Tamil Political Meme Classification

This repository contains the code for our submission to the **Multi Level Political Meme Classification - DravidianLangTech@ACL 2026** shared task (Tamil track).

Our system utilizes a late-fusion multimodal architecture to classify code-mixed Tamil political memes. We extract visual features using ResNet-50 and textual features using MuRIL, align them via Bidirectional Cross-Modal Attention, and fuse them using a Gated Multimodal Unit.

## Repository Contents
* `Gated_CrossModal_Hierarchical_XLSX_Polished.ipynb`: The main Jupyter Notebook containing the data loading, model architecture, training loop, and evaluation pipeline.

## Requirements
To run the notebook, you will need the following dependencies:
* `torch` and `torchvision`
* `transformers`
* `ocr_tamil`
* `openpyxl` and `pandas`
* `scikit-learn`
* `tqdm`

## Usage
1. Ensure the dataset (XLSX label files and meme images) is downloaded and placed in the appropriate directory.
2. Update the `TRAIN_EXCEL_PATH`, `TEST_EXCEL_PATH`, and `IMAGE_DIR_PATH` variables in the Configuration cell of the notebook.
3. Run all cells sequentially to execute the full hierarchical training and evaluation pipeline.

## Note on Dataset
The dataset used in this code was provided by the DravidianLangTech@ACL 2026 shared task organizers and is subject to their distribution rules.
