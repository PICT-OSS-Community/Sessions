# Simple Caluclator

A basic python package that provides basic calculatoe functionalities.


### Development Workflow with UV

#### Step 1: Initialize the Project with UV

1. **Install UV** (if not already):
```bash
pip install uv
```

2. **Initialize your project**:
Navigate to your project directory and initialize it with **UV**:
```bash
uv init
```

3. Add your dependencies to the `pyproject.toml` file created by uv


#### Step 2: Build the package:

command to build the package:
```bash
uv build
```
This command will create a `dist/` folder containing the built `.tar.gz` and `.whl` files.

#### Step 3: Install the package locally
```bash
uv pip install dist/calculator-0.1-py3-none-any.whl
```
Now you can test the calculator package by importing it in `test.py` file.

#### Step 4: Publish the Package
1. Use UV to publish your package directly to PyPI. Run:
```bash
uv publish
```
You may need to provide your PyPI credentials if publishing for the first time.

2. For the testing purposes, you can publish to the TestPyPI repository:
```bash
uv publish --repository testpypi
```



