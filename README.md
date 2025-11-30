# bv-live
ISO‑/live‑media builder and scripts: build‑scripts for Desktop, Gaming, Server, Cloud editions; overlays, branding, configs.

# 🛠 Contributing to Black Void Live

We welcome contributions from team members. To keep the repository clean and reproducible, please follow this workflow:

1. **Checkout the branch for your edition**
```bash
git checkout <edition-branch>
```
Example: `desktop-glibc`, `gaming-glibc`, `server-musl`, etc.

2. **Modify your files**
- Update **overlays** (wallpapers, icons, branding)
- Adjust **package lists** (`packages.txt`)
- Edit or improve **build scripts** (`build.sh`)

3. **Build locally**
```bash
./build.sh
```
- This generates a local ISO in your `out/` folder.
- Test the ISO in a VM to verify it boots and works correctly.

4. **Commit changes**
- Only commit **scripts, configs, overlays**, and other source files.
- **Do not commit ISO binaries** to the repository.

```bash
git add build-scripts/ overlays/ configs/
git commit -m "Update KDE config and wallpapers for 26.04 Desktop"
git push origin <edition-branch>
```

5. **Pull Request**
- Open a PR to merge your changes into `main`.
- Teammates review scripts and overlays before merging.
