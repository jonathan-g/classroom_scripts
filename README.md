# classroom_scripts
This repository holds simple scripts for interacting with GitHub classroom. I created these scripts for my own usage, and are making them public in case they help someone who is not used to scripting but who wants to use GitHub Classroom. 

To use: 

1. Download files
2. Copy files to the directory where you want to store, or have already stored, the repositories
3. Run the script using Terminal (on Mac) or Cygwin (on Windows). Each script has its own set of required parameters.

## classroom_clone: 

Clone all repositories for a given assignment into the current directory

* Requires a plaintext file with student usernames or group names, one name per line, ending with an empty line
* Parameter must be in this order:
  * Name of GitHub Classroom
  * Name of assignment
  * Name of file holding student usernames or groupnames
* Run with `sh classroom_clone.sh param1 param2 param3` where param1-3 are replaced with parameter values.

## classroom_push: 

Push changes to all directories in the current directory related to given assignment. There are two options: add a single file and commit/push (use if you create a gradesheet and just want to add it), or commit/push changes to all files in directory that are already added to the repository (use if you edit student code and want those comments to be pushed). Currently the commit message is hardcoded to be "Graded" but you can easily modify the script by changing "Graded" to your desired message before running.
