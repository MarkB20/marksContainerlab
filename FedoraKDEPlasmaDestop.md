# install docker 
````
sudo dnf install gnome-terminal
sudo dnf -y install dnf-plugins-core
sudo dnf config-manager --add-repo https://download.docker.com/linux/fedora/docker-ce.repo
sudo dnf install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
````

# start docker
````
sudo systemctl start docker
````
# install container labs 
````
# download and install the latest release (may require sudo)
bash -c "$(curl -sL https://get.containerlab.dev)"

# download a specific version - 0.10.3 (may require sudo)
bash -c "$(curl -sL https://get.containerlab.dev)" -- -v 0.10.3

# with wget
bash -c "$(wget -qO - https://get.containerlab.dev)"
````

# download vsCode
````
sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
sudo sh -c 'echo -e "[code]\nname=Visual Studio Code\nbaseurl=https://packages.microsoft.com/yumrepos/vscode\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/vscode.repo'

dnf check-update
sudo dnf install code # or code-insiders
````
