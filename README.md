## An introduction to QML in PennyLane and PyTorch (October 2025)
- **Author:** [Jacob Cybulski](https://jacobcybulski.com/) ([LinkedIn](https://www.linkedin.com/in/jacobcybulski/)), *Enquanted*
- **Collaboration with:**
      [Sebastian Zając](https://sebastianzajac.pl/) ([LinkedIn](https://www.linkedin.com/in/sebastianzajac/)),
      Tomasz Rybotycki ([LinkedIn](https://www.linkedin.com/in/tomasz-rybotycki-01192582/)) and
      Paweł Gora ([LinkedIn](https://www.linkedin.com/in/pawelgora/))
- **Associated with:** [QPoland](https://qworld.net/qpoland/) and [Quantum AI Foundation](https://www.qaif.org/)
- **Aims:** To explore the creation and use of quantum machine learning models in PennyLane (PL) and PyTorch.
- **Description:** This Quantum Machine Learning (QML) workshop provides an introduction to Quantum Machine Learning using PennyLane and PyTorch, with hands-on exercises and take-home challenges. The workshop includes four practical sessions that cover the QML concepts, models, and techniques. The sessions explore development of quantum estimators and classifiers, their training with various optimisers, loss and cost functions, as well as model testing and scoring using variety of metrics. It finally, explains how to create hybrid quantum-classical QML models.
- **Preparation:** Before attempting the workshop, we recommend to do some preparation first:
  - Download all resources (notes, code and data)
  - Install the recommended Python virtual environment (venv + requirements), see "install" folder
  - Undertake some preliminary exercises and get familiar with:
    - PyTorch, tensors, gradients and neural networks:<br>
      AssemblyAI, “PyTorch Crash Course - Getting Started with Deep Learning”, Jul 2022.<br>
      [https://www.youtube.com/watch?v=OIenNRt2bjg](https://www.youtube.com/watch?v=OIenNRt2bjg) (50 mins)
    - PennyLane, functions, circuits, qnodes and measurements:<br>
      Diego Emilio Serrano, “Basic Introduction to PennyLane”, Feb 2023.<br>
      [https://www.youtube.com/watch?v=MCDHAn-GvA8](https://www.youtube.com/watch?v=MCDHAn-GvA8) (40 mins)
    - PennyLane circuit creation and execution for busy people:<br>
      Isaac De Vlugt, “My first quantum circuit in PennyLane”, Sept 2023<br>
      [https://www.youtube.com/watch?v=uCm027_jvZ0](https://www.youtube.com/watch?v=uCm027_jvZ0) (5 mins)
    - Study two workshop notebooks in the "Explore" section (see table below) (1 hour)
    - You are now ready!
- **Structure:** Two preliminary self-study topics and four workshop sessions over two days, i.e.
  - _**Explore 1:**_ Self study (preliminary)
  - _**Explore 2:**_ Self study (preliminary)
  - _**Session 1:**_ QML foundation (basic)
  - _**Session 2:**_ Quantum estimators (intermediate)
  - _**Session 3:**_ Quantum classifiers (intermediate)
  - _**Session 4:**_ Hybrid models and QAEs (advanced)
- **Release Date:**
  - _**October, 10 2025:**_ The final versions will be made available 1 day before the workshop
- **Last Update:**
  - _**September 21, 2025:**_ Compatibility updates with recent versions of PennyLane and Torch.

### Important notebooks

You can play with these notebooks, enjoy!<br>
Note however that they may be updated at any time!

| Session | File | Description |
| :- | :- | :- |
| *Explore&nbsp;1* | s00_explore_tiny_model_vX_x.ipynb | Explains QML principles using PL |
| *Explore&nbsp;2* | s00_explore_meas_tests_vX_x.ipynb | Explains data encoding and measurements in PL |
|  |  |  |
| *Session&nbsp;1* | s01_simple_model_vX_x.ipynb | Creates and tests a very simple quantum model |
| *Session&nbsp;2* | s02_medium_qestimator_vX_x.ipynb | Creates and tests a more complex quantum estimator |
| *Session&nbsp;3* | s03_medium_qclassifier_vX_x.ipynb | (creates and tests a quantum classifier |
|  | s03_medium_cclassifier_vX_x.ipynb | Creates and tests a classical classifier |
| *Session&nbsp;4* | s04_advanced_hybrid_vX_x.ipynb | Creates and tests a quantum-classical hybrid model |
|  | s04_challenge_qae_vX_x.ipynb | Hard challenge to create a PyTorch quantum autoencoder |
|  |  |  |
| *Other* | utilities.py | A number of useful plotting functions to make your life easier |
| | requirements.txt | A list of software needed for this workshop (for auto-install with *pip*) |

### Folders
- _**notebooks:**_ all workshop notebooks can be found here
- _**images:**_ some images appearing in notebooks (via a relative link)
- _**legacy:**_ previous versions of files (in case you really really wanted them)
- _**slides:**_ presentation slides in PDF (as they become available)
- _**test:**_ test files are found here
  
### Requirements
- Set up a virtual environment with **venv** or **anaconda** for Python 3.11 and activate it
- Then install all software using **requirements.txt** file (available here):
    - pip install -r \<place-you-saved-it\>/requirements.txt
- Or install by hand by following these instructions:
    - pip install pennylane==0.42.3 pennylane-lightning==0.42.0 (PennyLane)
    - pip install scikit-learn==1.7.2 pandas==2.3.2 (ML)
    - pip install matplotlib==3.10.6 plotly==6.3.0 seaborn==0.13.2 pillow==11.3.0 (plots and images)
    - pip install jupyter==1.1.1 jupyterlab==4.4.7 (running jupyter notebooks)
    - pip install kagglehub==0.3.13 ucimlrepo==0.0.7 (data access)
    - pip install pdflatex (optionally to plot and export some plots and tables to latex)
    - install [PyTorch](https://pytorch.org/get-started/locally/), as per web site instructions, also add:<br>
      pip install torchvision torchaudio torchsummary torcheval torchmetrics

The **requirements.txt** file was tested for installation on 
Ubuntu 22.04-24.04, Windows 11 and MacOS Sequoia 15.3.1 (with M3 procesor).

### License
This project is licensed under the [GNU General Public License v3](./LICENSE).
The GPL v3 license requires attribution for modifications and derivatives, ensuring that users know which versions are changed and to protect the reputations of original authors.