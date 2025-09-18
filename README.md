This repository was forked from cvg/LightGlue. In order to use LightGlue in QGIS, we needed to get rid of the opencv dependency as opencv for Python>3.9 requires numpy>2, whereas QGIS till date (Version 3.41.10) is shipped with numpy==1.26.4. Accordingly, we replaced all opencv functionalities with scikit image. This further means, that currently SIFT and DoGHardNet are not available as they also depend on opencv.

Install this repo using pip:
```
git clone https://github.com/smfloery/LightGlue_QGIS.git && cd LightGlue_QGIS
python -m pip install -e .
```