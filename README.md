# 💻 Python Zip Cracker
Attempt cracking a proctected zip file using simple brute force.

This is a fun project to learn more about python modules, this project uses three:
- Tqdm: For the Progress Bar
- ZipFile: For working with zips
- PathLib: To check the validity of paths entered

```python
from pathlib import Path
from zipfile import ZipFile
from tqdm import tqdm
```

## File Structure
```python
root
  |--- zips/
    |--- secret.zip
  |--- script.py
```

## Running the script in your terminal
To actually run this script, you need a `wordlist` which is like a collection of passwords that we're going to cycle through and test against,
be sure to place this file in the root directory (or any folder in the root directory) and pass in the correct path to the text file in the terminal otherwise it won't work, you can use [this one](https://objects.githubusercontent.com/github-production-release-asset-2e65be/97553311/d4f580f8-6b49-11e7-8f70-7f460f85ab3a?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIWNJYAX4CSVEH53A%2F20221224%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20221224T171030Z&X-Amz-Expires=300&X-Amz-Signature=a12abea8ba4e37bf2daeb87e8a90fe7ccf0c36d0eed35c610fe08e4f8469c25a&X-Amz-SignedHeaders=host&actor_id=70282966&key_id=0&repo_id=97553311&response-content-disposition=attachment%3B%20filename%3Drockyou.txt&response-content-type=application%2Foctet-stream) [133 MB] containing about 14 million commonly used passwords stored in decreasing order of frequency

### My Folder Structure
<img width="960" alt="terminal - crack zip - 01" src="https://user-images.githubusercontent.com/70282966/209449723-a0713cbc-2ea4-4203-9971-c3ee638251bb.png">



I stored my `wordlist` text file which is called passwords in the root directory. I also have a zip in the `zips/` directory which I called __secret__.  
This command executes the script if you've added python to your __PATH VARIABLES__
```bash
~ python script.py

```

### Cracking the zip file
as you can see, I've cracked the zip file in just under **4 mins**. It's an unusual password, but it works  


<img width="960" alt="terminal - crack zip - 02" src="https://user-images.githubusercontent.com/70282966/209449696-1986ef9d-86d5-4aeb-9f33-150310fc2580.png">

<img width="960" alt="extracting zip" src="https://user-images.githubusercontent.com/70282966/209449896-a3cb306b-55bb-430f-bdd3-229f0046003d.png">
<img width="960" alt="extracted zip" src="https://user-images.githubusercontent.com/70282966/209449899-14fbe6c7-8417-477e-a35b-eed475865039.png">

## Disclaimer
This project was made to learn more about python libraries and modules, it's not intended to be used in any malicious way. **You're responsible** for how you chose to use the script.  
Made with python and ☕  
### ⭐ Star this repo if you like this project







