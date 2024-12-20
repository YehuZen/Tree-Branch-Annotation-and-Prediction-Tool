<div align="center">
  <img src="assets/logo.png" alt="Tree Branch Tool Logo" width="200" height="200"/>

  # **🌳 Tree Branch Annotation and Prediction Tool**

  *A Comprehensive Tool for Annotating and Predicting Tree Branch Structures*

  [**📄 Read the Paper**](https://doi.org/10.3390/f15091659) | [**🔽 Download Pre-trained Models**](models/) | [**📂 Explore Dataset**](data/)
</div>

---

## **📖 Introduction**

This repository provides **two versions** of the **Tree Branch Annotation Tool**:

### 1. **Tree Branch Annotation Tool (No Prediction)**
A simple tool for **manually annotating tree branches** (main trunks and side branches) on RGB images.

### 2. **Tree Branch Annotation and Prediction Tool**
A more advanced version of the tool that includes all features from the first tool, plus **deep learning-based prediction** for tree branch structures using pre-trained models.

Both versions are developed for the research paper:  
[**Automatic Method for Extracting Tree Branching Structures from a Single RGB Image**](https://doi.org/10.3390/f15091659) (**doi: 10.3390/f15091659**).

---

## **✨ Features**

### **1. Tree Branch Annotation Tool (No Prediction)**

✅ **Interactive Annotation**  
Manually annotate **main trunks** and **side branches** with ease.

✅ **Save and Export**  
Save annotated points as structured XML files for future use.

### **2. Tree Branch Annotation and Prediction Tool**

✅ **Deep Learning Prediction**  
After annotating the main trunk and branches, use pre-trained models to predict additional tree branch points.

✅ **Interactive Annotation and Prediction**  
Annotate and then predict tree branch structures, both using deep learning models.

---

## **🖱️ Usage Instructions**

### **For the Tree Branch Annotation Tool (No Prediction)**

1. **Open the Image**:  
   Click the **"Open File"** button to load an image.

2. **Annotate the Main Trunk**:  
   - Set the right panel mode to **"Main Branch"**.
   - Left-click to annotate the **main trunk**.
   - Once finished, click **"Draw Line"** to connect the points.

3. **Annotate the Side Branch**:  
   - Change the right panel mode to **"Sub-Branch"**.
   - Right-click to annotate **side branches**.

4. **Save the Annotations**:  
   - Click **"Save Annotations"** to save your work as an XML file.

---

### **For the Tree Branch Annotation and Prediction Tool**

1. **Open the Image**:  
   Click **"Open File"** to load an image for annotation.

2. **Annotate the Main Trunk**:  
   - Set the right panel mode to **"Main Branch"**.
   - Left-click to annotate the **main trunk**.
   - Once finished, click **"Draw Line"** to connect the points.

3. **Annotate the Side Branch**:  
   - Change the right panel mode to **"Sub-Branch"**.
   - Right-click to annotate **side branches**.

4. **Save the Annotations**:  
   - After completing annotations, click **"Save Annotations"** to save your work as an XML file.

5. **Load a Model and Predict**:  
   - After opening an image, click **"Select Model"** to load a pre-trained model.
   - Click **"Predict"** to predict tree branch points using the model.

---

## **📁 Pre-trained Models**

Two pre-trained models are available for **prediction**:

- **Model (399_checkpoint.pth)**: Trained for **400 epochs**, providing moderate accuracy.
- **Model (1199_checkpoint.pth)**: Trained for **1200 epochs**, providing higher accuracy.


---

## **📊 Sample Dataset**

The repository includes a small, **CreativeML Open RAIL++-M** dataset for testing:

- Located in the [data/](data/) directory.
- Includes sample images and corresponding XML annotations.

---

## **📂 Project Structure**

```plaintext
tree-branch-annotation/
│
├── data/                # Data directory (datasets, images, XML files)
│   ├── xml/             # Saved XML files
│   ├── png/             # Annotated images
│
├── 399_checkpoint.pth    # Pre-trained models 400 epochs
├── 1199_checkpoint.pth   # Pre-trained models 1200 epochs
│
├── LabelPredictor.py       # For the Tree Branch Annotation and Prediction Tool
├── Label.py                # No Prediction
├── requirements.txt     # Python dependencies
├── README.md            # Documentation
```

---

## **📜 Citing this Work**

If you use this tool in your research, please cite the following paper:

**Automatic Method for Extracting Tree Branching Structures from a Single RGB Image**  
[DOI: 10.3390/f15091659](https://doi.org/10.3390/f15091659)

```bibtex
@Article{f15091659,
AUTHOR = {Yang, Yinhui and Lai, Huang and Chen, Bin and Huo, Yuchi and Xia, Kai and Huang, Jianqin},
TITLE = {Automatic Method for Extracting Tree Branching Structures from a Single RGB Image},
JOURNAL = {Forests},
VOLUME = {15},
YEAR = {2024},
NUMBER = {9},
ARTICLE-NUMBER = {1659},
URL = {https://www.mdpi.com/1999-4907/15/9/1659},
ISSN = {1999-4907},
DOI = {10.3390/f15091659}
}

