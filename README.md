# pycocotools-fix

The original [cocoapi](https://github.com/cocodataset/cocoapi) package installaion fails if cython or numpy is not installed. This constraints makes automated dependency management difficult, as pip needs to be called twice, first to install cython and numpy, and then second time to install pycoco. This repository fixed the dependency constraint so that pycoco can be installed with a single run of pip.

This fix is published to pypi as [pycocotools-fix](https://pypi.org/project/pycocotools-fix/), since the original repository is no longer maintained. To install, use the following command.

```
pip install pycocotools-fix
```


## Original README
COCO API - http://cocodataset.org/

COCO is a large image dataset designed for object detection, segmentation, person keypoints detection, stuff segmentation, and caption generation. This package provides Matlab, Python, and Lua APIs that assists in loading, parsing, and visualizing the annotations in COCO. Please visit http://cocodataset.org/ for more information on COCO, including for the data, paper, and tutorials. The exact format of the annotations is also described on the COCO website. The Matlab and Python APIs are complete, the Lua API provides only basic functionality.

In addition to this API, please download both the COCO images and annotations in order to run the demos and use the API. Both are available on the project website.
-Please download, unzip, and place the images in: coco/images/
-Please download and place the annotations in: coco/annotations/
For substantially more details on the API please see http://cocodataset.org/#download.

After downloading the images and annotations, run the Matlab, Python, or Lua demos for example usage.

To install:
-For Matlab, add coco/MatlabApi to the Matlab path (OSX/Linux binaries provided)
-For Python, run "make" under coco/PythonAPI
-For Lua, run “luarocks make LuaAPI/rocks/coco-scm-1.rockspec” under coco/
