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
  ```
gcloud cloud-shell ssh --authorize-session --command="go install -v github.com/projectdiscovery/nuclei/v3/cmd/nuclei@latest"
```
## isntall go (first then nuclei)
```
gcloud cloud-shell ssh --authorize-session --command="sudo apt update && sudo apt install -y golang-go && go install -v github.com/projectdiscovery/nuclei/v3/cmd/nuclei@latest && echo 'export PATH=\$PATH:\$HOME/go/bin' >> ~/.bashrc && source ~/.bashrc && ~/go/bin/nuclei -version"
```
## 🚀 Cara Menggunakan:
### Untuk menggunakan Nuclei di Cloud Shell, gunakan path lengkap:
```
~/go/bin/nuclei [options]
```
## or

```
# Scan single target
~/go/bin/nuclei -u example.com

# Scan dengan template tertentu
~/go/bin/nuclei -u example.com -t http/cves/

# Update templates
```
~/go/bin/nuclei -update-templates
```
# Examples
## Menggunakan testphp.vulnweb.com (situs khusus untuk testing)
```
```
gcloud cloud-shell ssh --authorize-session --command="~/go/bin/nuclei -u http://testphp.vulnweb.com"
```
```
## Menggunakan DVWA (Damn Vulnerable Web Application)

```
gcloud cloud-shell ssh --authorize-session --command="~/go/bin/nuclei -u http://dvwa.co.uk"
```

## Menggunakan localhost/lab environment sendiri

```
gcloud cloud-shell ssh --authorize-session --command="~/go/bin/nuclei -u http://localhost"
```
---



