
<p align="center">
<img src="https://github.com/mayHamad/AutoParser/assets/46843593/937423e9-5478-4cd6-b838-02bddcbd60d5" width=30% height=30% >
<p />

# AutoParser
AutoParser is a forensic tool for parsing offline registry hives in order to extract forensic artifacts, which includes auto startup programs, lateral movement, archive files history, and other valuable artifacts.

# Features
- Parse offline registry hives.
- Replay transaction logs against the hive.
- Provide the timestamps of Windows registry keys creation.
- Compatible with the [Kuiper](https://github.com/DFIRKuiper/Kuiper) platform.
- Support multiple output formats (CSV and JSON).

# How to use
- Install Python 3
- Install tool's dependences:
```
pip3 install -r requirment.txt
```
# Example
Below command will pares with all plugins using '-a' switch:
```
python3 AutoParser.py -a -p [path to folder of all registry hives] -o [path to results folder]
```
- The results will be in folder that specified in command and each plugin results will be in separate file.

# Licences
this project depends on:
- YARP https://github.com/msuhanov/yarp
- RegSkewer https://github.com/muteb/RegSkewer

# Refernces
https://www.microsoftpressstore.com/articles/article.aspx?p=2762082&seqNum=2
