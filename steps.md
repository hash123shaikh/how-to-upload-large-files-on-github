# Step-by-Step: Upload Big Files on GitHub

## 1. Install Git LFS (only once)

### For Linux:
```bash
sudo apt update
sudo apt install git-lfs
git lfs install

For Windows:
- Go to: https://git-lfs.github.com
- Download and install
- Then open Git Bash and run: git lfs install

## 2. Track big files
This tells Git to use LFS for your large files:

git lfs track "*.mp4"
git lfs track "*.dcm"

This creates a `.gitattributes` file.

## 3. Upload your files
Now upload like this:

git add .
git commit -m "add files"
git push origin main
