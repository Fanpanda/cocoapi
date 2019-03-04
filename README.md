To support Windows build and python3 we had to make [minor changes](https://github.com/cocodataset/cocoapi/compare/master...philferriere:master#diff-49ecc5c8e93163121e2cc2eb6b1fca2c) to:

- `PythonAPI/setup.py`
- `PythonAPI/pycocotools/coco.py`

To install this package, use `pip` as follows:

```
pip install git+https://github.com/philferriere/cocoapi.git#subdirectory=PythonAPI
```
Info
```
Collecting git+https://github.com/philferriere/cocoapi.git#subdirectory=PythonAPI
  Cloning https://github.com/philferriere/cocoapi.git to c:\users\phil\appdata\local\temp\pip-req-build-jn698z8p
Building wheels for collected packages: pycocotools
  Running setup.py bdist_wheel for pycocotools ... done
  Stored in directory: C:\Users\Phil\AppData\Local\Temp\pip-ephem-wheel-cache-rde3oevt\wheels\69\2b\12\2fa959e49f73d26cff202c2f4e5079096c9c57c8a8509fd75c
Successfully built pycocotools
Installing collected packages: pycocotools
Successfully installed pycocotools-2.0
```

On Windows, you must have the Visual C++ 2015 build tools on your path. If you don't, make sure to install them from [here](https://go.microsoft.com/fwlink/?LinkId=691126):

![](img/download.png)

Then, run `visualcppbuildtools_full.exe` and select default options:

![](img/install.png)
