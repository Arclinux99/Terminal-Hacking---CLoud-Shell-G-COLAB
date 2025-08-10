# Terminal-Hacking---CLoud-Shell-G-COLAB
if you want to more secure when hacking, this is for you. 

```ad-quote
gcloud cloud-shell ssh --command="sudo -i"
```
```
gcloud cloud-shell ssh --command="sudo pacman -Sy"
```
---
## nuclei installaltion
  gcloud cloud-shell ssh --authorize-session --command="go install -v github.com/projectdiscovery/nuclei/v3/cmd/nuclei@latest"

## isntall go (first the nuclei)
gcloud cloud-shell ssh --authorize-session --command="sudo apt update && sudo apt install -y golang-go && go install -v github.com/projectdiscovery/nuclei/v3/cmd/nuclei@latest && echo 'export PATH=\$PATH:\$HOME/go/bin' >> ~/.bashrc && source ~/.bashrc && ~/go/bin/nuclei -version"

## 
