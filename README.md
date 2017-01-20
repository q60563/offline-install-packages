# offline-install-packages

# Download packages.deb
- 在連線裝置下執行以下指令下載packages
```
$sudo apt-get --download-only install packagesname
```
- 下載後位置存放在
```
$cd /var/cache/apt/archives
```
- 將deb檔存放至離線裝置執行以下指令進行安裝（path）為存放路徑
```
$sudo dpkg -i /path/*.deb
```

# Download packages.tar.gz
- 在連線裝置下執行以下指令下載packages
```
$sudo pip install --download /path packagesname 
```
- 將tar.gz檔存放至離線裝置執行以下指令進行安裝（path）為存放路徑
```
$sudo pip install --no-index --find-links=file:/path packagesname
```