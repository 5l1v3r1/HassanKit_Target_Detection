# Targeted #HassanKit Attack User Validation 
### UPDATE: I have since removed this opendir for obfuscation & TLP reasons, those with access to the list... Add all directory path URLs containing to urls.txt line by line like shown in the file.

This script automates the checking of users contained within the targeted attack dumps.

*I recommend running in a sandbox/off network environement*

### To use: 
```sh
$ git clone https://github.com/littl3field/HassanKit_Target_Detection
```
```sh
$ cd HassanKit_Target_Detection
$ sudo pip install -r requirements.txt
```
Run you query like this to check if your organisation or search term is within the dataset. Example below uses "companyname" as the arguement. At this moment, it is case sensitive, so please use lower case. 
```sh
$ python VALIDATE.py companyname
```

### Output: 
- result.txt = full list of data collected from the server
- matches.txt = all users matched within the dataset

Note: If not all data is grabbed it might be a bandwidth issue. I'll improve the effiency soon.
This is a quick bodge script to automate the task right now. I'll improve it if the attack continues.
