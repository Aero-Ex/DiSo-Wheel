# DiSo-Wheel

GitHub Actions repository to build `diso` wheels for specific CUDA and PyTorch versions.

## How to use
1. Push this repository to a new GitHub repo.
2. The workflow will automatically trigger on push to `main` or `master`.
3. Check the **Actions** tab on GitHub to monitor the build.
4. Once finished, download the wheel from the **Artifacts** section.
5. Install the wheel in your `comfyvenv` using:
   ```bash
   pip install path/to/diso-0.1.4-cp311-cp311-linux_x86_64.whl
   ```

## Local Push Commands
If you have the `gh` CLI installed:
```bash
gh repo create DiSo-Wheel --public --source=. --remote=origin --push
```
Or manually:
```bash
git add .
git commit -m "Initial commit: Add wheel builder workflow"
git remote add origin https://github.com/YOUR_USERNAME/DiSo-Wheel.git
git push -u origin master
```
