# Command line
| Command      | Explanation             |
| ------------ | ----------------------- |
| Ctrl+Shift+c | Copy command line texts |
| Ctrl+Shift+v | Past command line texts | 


# Working directory
| Command                                 | Explanation                                                                                                                     |
| --------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- |
| pwd                                     | Retrieve current working directory                                                                                              |
| mkdir ~/BIO214/LabPractical1/testfolder | Create a directory called testfolder with mkdir (`~` and `.` are used to represent the home directory (/Users/YOUR_USER_NAME/)) |
| cd ~/BIO214/LabPractical1/testfolder    | Change the current working directory toward the folder with cd                                                                  |
| rm -r ~/BIO214/LabPractical1/testfolder | Remove the entire test folder with rm                                                                                           | 



# Files
| Command                                             | Explanation                                                           |
| --------------------------------------------------- | --------------------------------------------------------------------- |
| ls                                                  | List all the files/floders in current working directory               |
| ls -lh                                              | Return more file information (file size, date of change, file access) |
| mv Helloworld.txt ~/BIO214/LabPractical1/testfolder | Move the file toward the folder with mv                               | 


## File content operation
| Command                                                | Explanation                                                                                     |
| ------------------------------------------------------ | ----------------------------------------------------------------------------------------------- |
| echo This is my first file > Helloworld.txt            | Create a text message with content 'This is...' and store it in a file named by 'Hellowrld.txt' |
| cat Hellowrld.txt                                      | Check the content of Helloworld.txt                                                             |
| head -n 12 SRR1039508_sub_1.fastq                      | Check the first 12 lines of the file                                                            |
| head -n 10 SRR1039508_1.fastq > SRR1039508_sub_1.fastq | Write the first 10 lines to a new file                                                          |

## Extract & install tar.gz files
- Download the desired .tar.gz or (.tar.bz2) file
- Open Terminal
- Extract the .tar.gz or (.tar.bz2) file with the following commands:
	```bash
	tar xvzf PACKAGENAME.tar.gz
	tar xvjf PACKAGENAME.tar.bz2
	```
- Nevigate to the extracted folder using `cd` command
	```bash
	cd PACKAGENAME
	```
- Now run the following command to install the tarball
	```bash
	./configure
	make
	sudo make install
	```

### Example with hg19 index
```bash
cd data/hg19_idx/genome
wget https://genome idx.s3.amazonaws.com/hisat/hg19_genome.tar.gz
tar xvzf hg19_genome.tar.gz
```






