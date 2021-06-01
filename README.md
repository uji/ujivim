# ujivim

## download vim distribution

```
curl -s https://api.github.com/repos/uji/ujivim/releases/latest \
| grep "browser_download_url.*linux-amd64.tar.gz" \
| cut -d : -f 2,3 \
| tr -d \" \
| xargs curl -o ujivim.tar.gz -L
```
