# WWR

## How to Run
### Prerequisites
1. **Install Python**: Ensure you have Python 3.8 or later installed. You can download it from [Python.org](https://www.python.org/).

2. **Clone the Repository**:
   ```
   git clone https://github.com/mohamadalbaaj/WWR.git
   ```
   ```
   cd WWR
   ```

3. **Set Up a Virtual Environment (optional but recommended)**:
   ```
   python -m venv venv
   ```
   ```
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```
4. **Install Dependencies**:
   ```
   pip install -r requirements.txt
   ```
5. **Install Jupyter (if not already installed)**:
   ```
   pip install notebook
   ```   
### Open Notebooks
1. **Open the Relevant Notebook**:
- **object_detection_fasterrcnn.ipynb**  
  For object detection using Faster R-CNN  

- **semantic_segmentation_fcnresnet.ipynb**  
  For semantic segmentation using FCN ResNet
2. **Configure Notebook Environment**:
- Before running the cells, verify that the kernel is set to the virtual environment you created earlier.
- Click Kernel > Change Kernel and select your environment.
3. **Execute Cells**:
- Run All: Click Cell > Run All in the toolbar

## Citation
this project uses dataset provided by:

(https://github.com/lck1201/win_det_heatmaps.git)

```
@article{Chuan-Kang Li:900, 
    author = {Chuan-Kang Li, Hong-Xin Zhang, Jia-Xin Liu, Yuan-Qing Zhang, Shan-Chen Zou, Yu-Tong Fang},
    title = {Window Detection in Facades Using Heatmap Fusion},
    publisher = {Journal of Computer Science and Technology},
    year = {2020},
    journal = {Journal of Computer Science and Technology},
    volume = {35},
    number = {4},
    eid = {900},
    numpages = {12},
    pages = {900},
    keywords = {facade parsing;window detection;keypoint localization},
    url = {http://jcst.ict.ac.cn/EN/abstract/article_2660.shtml},
    doi = {10.1007/s11390-020-0253-4}
}  
```
