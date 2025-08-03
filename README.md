# LibreGrad RootFS

Custom root filesystem for LibreGrad Linux distribution. No BusyBox, fully from scratch.

## ✅ Purpose
Implements:
- Custom init system
- Core utilities
- Minimal system layout

## 📂 Structure
- `src/init/` → Init system
- `src/utils/` → Core utilities (ls, cat, echo)
- `rootfs/` → Generated root filesystem
- `scripts/` → Build and packaging scripts
- `Dockerfile` → Build container

## 🚀 Build Instructions
```bash
make build   # Compiles init + utilities, assembles rootfs
make package # Creates initramfs or tarball
