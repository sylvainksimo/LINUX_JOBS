# Perform Fedora Update

```sh
sudo dnf update
```

# Add GPG key and Repository (using ShiftKey or mirror MWT RPM package repositories): mirror MWT is recommended

```sh
sudo rpm --import https://mirror.mwt.me/shiftkey-desktop/gpgkey
sudo sh -c 'echo -e "[mwt-packages]\nname=GitHub Desktop\nbaseurl=https://mirror.mwt.me/shiftkey-desktop/rpm\nenabled=1\ngpgcheck=1\nrepo_gpgcheck=1\ngpgkey=https://mirror.mwt.me/shiftkey-desktop/gpgkey" > /etc/yum.repos.d/mwt-packages.repo'
sudo rpm --import https://rpm.packages.shiftkey.dev/gpg.key
sudo sh -c 'echo -e "[shiftkey-packages]\nname=GitHub Desktop\nbaseurl=https://rpm.packages.shiftkey.dev/rpm/\nenabled=1\ngpgcheck=1\nrepo_gpgcheck=1\ngpgkey=https://rpm.packages.shiftkey.dev/gpg.key" > /etc/yum.repos.d/shiftkey-packages.repo'
```


# Run the system update command to rebuild the DNF package manager cache

```sh
sudo dnf update
```

# Installing GitHub Desktop client on Fedora (with yum OR dnf)

```sh
sudo yum install github-desktop
sudo dnf install github-desktop
```

# Open GitHub Desktop

```sh
github-desktop
```
