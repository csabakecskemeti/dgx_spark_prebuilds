# Prebuilt FFmpeg for DGX Spark (ARM64)

This folder contains a prebuilt FFmpeg installation for DGX Spark (ARM64).

## Download and Extract

You can download the prebuilt FFmpeg tarball and extract it directly to `/usr/local/ffmpeg`:

```bash
# Download the prebuilt FFmpeg tarball
wget https://github.com/csabakecskemeti/dgx_spark_prebuilds/raw/main/ffmpeg/ffmpeg-arm64-prebuilt.tar.gz -O /tmp/ffmpeg-arm64-prebuilt.tar.gz

# Extract to /usr/local (requires sudo)
sudo tar -xzvf /tmp/ffmpeg-arm64-prebuilt.tar.gz -C /usr/local
```

Add FFmpeg to Your Environment

```bash
# Add FFmpeg library path
export LD_LIBRARY_PATH=/usr/local/ffmpeg/lib:$LD_LIBRARY_PATH

# Add FFmpeg binaries to PATH
export PATH=/usr/local/ffmpeg/bin:$PATH
```

Verification

Check that FFmpeg is installed correctly:

```bash
ffmpeg -version
```

## Notes
This prebuilt FFmpeg is for ARM64 DGX Spark systems.
