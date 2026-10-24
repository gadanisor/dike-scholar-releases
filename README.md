# Dike Scholar Releases

This repository contains Dike Scholar release assets and the signed APT
repository served from `https://repo.dike.ro`.

## Install on Debian or Ubuntu

```bash
curl -fsSL https://repo.dike.ro/dike-archive-keyring.gpg \
  | sudo tee /usr/share/keyrings/dike-scholar-archive-keyring.gpg >/dev/null

echo "deb [arch=amd64 signed-by=/usr/share/keyrings/dike-scholar-archive-keyring.gpg] https://repo.dike.ro stable main" \
  | sudo tee /etc/apt/sources.list.d/dike-scholar.list

sudo apt update
sudo apt install dike-scholar
```

Supported operating systems: Windows, macOS, and Linux.
