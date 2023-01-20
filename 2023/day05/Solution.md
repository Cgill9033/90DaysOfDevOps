Tasks:

Write a bash script createDirectories.sh that when the script is executed with three given arguments (one is directory name and second is start number of directories and third is the end number of directories ) it creates specified number of directories with a dynamic directory name.
When the script is executed as ./createDirectories.sh Movie 20 50 then it creates 50 directories as Movie20 Movie21 Movie23 ...Movie50

#!/bin/bash

#mkdir creates a directory
#$1 $2 $3 ar arguments in this case (Movie , 20, 50)

mkdir -p $1{$2..$3}

#To run press run ./createDirectories.sh Movie 20 50


----------------------------------------------------------------------------------------------
Create a Script to backup all your work done till now.
#!/bin/bash

# Set the current date and time
now=$(date +"%Y-%m-%d-%H-%M-%S")

# Create a backup of the directory "honey"
tar -zcf honey_backup_$now.tar.gz honey/

# Print a message to confirm the backup was created
echo "Backup of honey created successfully as honey_backup_$now.tar.gz"

-------------------------------------------------------------------------------------------------

Create 2 users and just display their Usernames
sudo useradd user1
sudo useradd user2

id user1 / id -un user1
id user2 / id -un user2
