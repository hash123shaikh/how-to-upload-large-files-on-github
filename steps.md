# Step-by-Step: Upload Big Files on GitHub

## 1. Install Git LFS (only once)

### For Windows:
- Go to: https://git-lfs.github.com
- Download and install Git LFS
- Then open Git Bash and run:

```bash
git lfs install
```

## 2. Track big files
Tell Git to use LFS for your big files:

```bash
git lfs track "*.mp4"
git lfs track "*.dcm"
```
This creates a `.gitattributes` file.

## 3. Upload your files
Now upload your files like normal:

```bash
git add .
git commit -m "add files"
git push origin main
```

## ✅ Notes:

- Max file size = 2 GB

- Git LFS free = 1 GB storage + 1 GB/month download

- For files bigger than 2 GB → use Google Drive, Dropbox, or Zenodo and just add the download link in your README.

