# Prebuilt Decord for DGX Spark (ARM64, Python 3.12)

This folder contains a prebuilt Decord wheel for ARM64, compatible with Python 3.12 on DGX Spark.

## Installation

You can install the prebuilt Decord directly from this GitHub repository:

```bash
# Activate your Python virtual environment first
source /path/to/your/venv/bin/activate

# Install Decord directly from GitHub
pip install https://github.com/csabakecskemeti/dgx_spark_prebuilds/raw/main/decord/decord-0.6.0-cp312-cp312-linux_aarch64.whl
```

## Verification

After installation, verify that Decord is available:

```bash
python -c "import decord; print(decord.__version__)"
# Expected output: 0.6.0
```
## Notes
- This wheel is precompiled for ARM64 architecture and CUDA-ready DGX Spark environments. 
- Ensure you are using Python 3.12 in your virtual environment.
