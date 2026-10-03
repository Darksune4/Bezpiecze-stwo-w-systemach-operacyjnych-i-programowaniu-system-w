**Temat:** 1. Piaskownica procesowa w Linuksie: przestrzenie nazw, cgroups i seccomp
---
### Eksperyment 1: Przestrzenie nazw 
* **Wykonane polecenie:** `sudo unshare --pid --fork --mount-proc bash` oraz `ps aux`
  <img width="1006" height="197" alt="изображение" src="https://github.com/user-attachments/assets/ac54adfe-09cc-4caf-9504-2d11c5c7b18c" />

### Eksperyment 2: Ograniczenie zasobów
* **Wykonane polecenie:** `systemd-run --user --scope -p MemoryMax=100M bash` a następnie obciążenie procesora komendą `yes > /dev/null`.
  <img width="1008" height="222" alt="изображение" src="https://github.com/user-attachments/assets/68c2d2a8-f0a8-4ba5-8d36-5595f1e126ae" />
