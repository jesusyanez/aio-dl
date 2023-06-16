# Universal File Fetcher

#### <p><i>Download from Google Drive, MediaFire, Dropbox, or WeTransfer.</i></p>



- Python 3
- Works on all operating systems
- No APIs needed
- Auto extracts .zip & .rar folders (rar requires 7zip) 
- Removes all compressed files after extraction

## Supported Link Formats

### Google Drive
```txt
https://drive.google.com/drive/folders/example?usp=sharing
https://drive.google.com/file/d/example/view?usp=sharing
```

### Dropbox
```txt
https://www.dropbox.com/s/example/example?dl=0
https://www.dropbox.com/sh/example/example?dl=0
https://www.dropbox.com/s/example/example?dl=1
https://www.dropbox.com/sh/example/example?dl=1
```
### MediaFire
```txt
https://www.mediafire.com/file/example/example/file
```
### WeTransfer
```txt
https://wetransfer.com/downloads/example/example
```

## Usage

```python3
import cdl

url1 = "https://drive.google.com/drive/folders/example?usp=sharing"
url2 = "https://www.dropbox.com/s/example/example?dl=0(1)"
url3 = "https://www.mediafire.com/file/example/example/file"
url4 = "https://wetransfer.com/downloads/example/example"

download_list = [url1, url2, url3, url4]
download_path = "./downloads/" #make sure this directory already exists

for url in download_list:
 cdl.grab(url, download_path)
```

## Roadmap

- [x] Google Drive
- [x] Dropbox
- [x] MediaFire
- [x] WeTransfer
- [ ] Mega

## Acknowledgement

Code was borrowed from <a href="https://github.com/matthuisman/gdrivedl">gdrivedl</a>, <a href="https://github.com/Juvenal-Yescas/mediafire-dl">mediafire-dl</a>, and <a href="https://github.com/iamleot/transferwee">transferwee</a> to create lootdl.
