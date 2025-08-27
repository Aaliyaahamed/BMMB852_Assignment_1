# BMMB 852: Assignment_1

## 1. Samtools Version in Bioinfo Environment

**Input:**
```bash
conda activate bioinfo
samtools --version
```

**Output:**
```bash
samtools 1.15.1
Using
```



## 2. Creating a nested directory structure
**Input:**
```bash
mkdir -p assignment1/testdata/rawdata
ls -R assignment1
```

**Ouput:**
``` bash
assignment1:
testdata

assignment1/testdata:
rawdata

assignment1/testdata/rawdata:

```
## 3. Creating files in directories
**Input:**

```bash
touch assignment1/testdata/rawdata/file1.txt
touch assignment1/testdata/rawdata/file2.txt
touch assignment1/testdata/info.txt
touch assignment1/notes.txt
ls -R assignment1
```

**Ouput:**
``` bash
assignment1:
notes.txt  testdata

assignment1/testdata:
info.txt  rawdata

assignment1/testdata/rawdata:
file1.txt  file2.txt
```
## 4. Relative and Absolute Paths
**Input:**
``` bash
# File in assignment1
cat assignment1/notes.txt

# File in testdata
cat assignment1/testdata/info.txt

# Files in rawdata
cat assignment1/testdata/rawdata/file1.txt
cat assignment1/testdata/rawdata/file2.txt
```

**Ouput:**
``` bash
This is my notes file
This is info file in testdata
This is file1 in rawdata
This is file2 in rawdata
```

**Input:**
``` bash
cat /mnt/d/BMMB_F2026/assignments/BMMB-852--Assignment_1/assignment1/notes.txt
cat /mnt/d/BMMB_F2026/assignments/BMMB-852--Assignment_1/assignment1/testdata/info.txt
cat /mnt/d/BMMB_F2026/assignments/BMMB-852--Assignment_1/assignment1/testdata/rawdata/file1.txt
cat /mnt/d/BMMB_F2026/assignments/BMMB-852--Assignment_1/assignment1/testdata/rawdata/file2.txt
```
**Ouput:**
``` bash
This is my notes file
This is info file in testdata
This is file1 in rawdata
This is file2 in rawdata
```






