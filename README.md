<h4 align="center"> Removing CDN IPs from the list of IP addresses </h4>
<p align="center">
  <a href="#cdn-providers">CDN Providers</a> •
  <a href="#installation">Install</a> •
  <a href="#usage-parameters">Usage Parameters</a> •
  <a href="#preview">Preview</a> •
  <a href="#usage">Usage</a> •
  <a href="https://t.me/ImAyrix">Contact me</a>
</p>

---

The tool's basic functionality would involve taking the list of IP addresses as input and then checking to determine whether the IP is behind a CDN.
This tool will gather all CIDR of the most-known CDN providers and check your provided list with them.
This is a handy tool for bug hunters.

## CDN Providers
* Akamai
* Amazon
* Arvancloud
* Azure CDN
* Bing
* Cloudflare
* Cloudfront
* DDoS Guard
* Digitalocean
* Fastly
* Google cloud
* Incapsula
* Leaseweb
* Maxcdn
* Oracle
* Qrator
* StackPath
* StormWall
* Sucuri
* X4B

# Installation

#### From Source
```bash
 go install github.com/PushkraJ99/cut-cdn@latest

```

#### From GitHub:
```bash
git clone github.com/PushkraJ99/cut-cdn
cd cut-cdn; go build
sudo mv cut-cdn /usr/local/bin

cut-cdn
```
- Now you can use cut-cdn as any other Linux Tool from any Terminal without opening tool clone Directory / Folder


## Usage Parameters
```
  -c string
        Use cache file (offline) [Path]
  -i string
        Input [Filename | IP]
  -o string
        Output [Filename] (default "terminal")
  -s string
        Save all cidr [Path]
  -silent
        show only IPs in output
  -t int
        Number Of Thread [Number] (default 1)
```

## Preview

![cut-cdn](https://user-images.githubusercontent.com/89543912/221229391-5bb70bb1-5b6f-43ae-a912-0d1663498cad.png)

## Usage


### Online mode
Check your IP list with the latest IP ranges of CDN providers:

+ Single IP
    ```bash 
    cut-cdn -i 127.0.0.1
    echo "127.0.0.1" | cut-cdn
    ```
+ List of IPs
    ```bash
  cut-cdn -i allIP.txt
  cat allIP.txt | cut-cdn
    ```
+ To store results use `-o` option
    ```bash
    cut-cdn -i allIP.txt -o output.txt
    ```
+ To set concurrency use -t option (Default is 1)
  ```bash
  cut-cdn -i allIP.txt -o output.txt -t 20
  ```
### Offline mode
1. To check IPs in offline mode you should save CDNs IP ranges in a file
    ```bash
    cut-cdn -s allCIDR.txt
   ```
2. After that you can run it in offline mode by `-c` pointing to the CIDR file
    ```bash
   cut-cdn -i allIP.txt -o output.txt -t 20 -c allCIDR.txt
   ```


## 🌐 Socials : Follow Me Here For More

[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://instagram.com/you_are_not_goodlooking_but_he)

[![Twitter](https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/intent/follow?screen_name=PushkraJ99) 

[![Github](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/PushkraJ99)

[![TryHackMe](https://img.shields.io/badge/TryHackMe-%23D42029.svg?logo=TryHackMe&logoColor=white)](https://tryhackme.com/p/PushkaraJ)



## [Snake4Readme](https://github.com/PushkraJ99/Snake4Readme)

<p align="center">
<img src="https://github.com/PushkraJ99/Snake4Readme/blob/main/Snake4Readme/grid-snake.svg">
</p><br>

[![](https://visitcount.itsvg.in/api?id=PushkraJ99&icon=8&color=12)](https://visitcount.itsvg.in)

<p align="center"> 
  <b> Visitor count</b><br>
  <img src="https://profile-counter.glitch.me/PushkraJ99/count.svg" />
</p><br>
