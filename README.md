# rclone
#intall
curl https://rclone.org/install.sh | sudo bash

upload or sync with large file
 rclone --transfers=32 --checkers=16 --drive-chunk-size=16384k --drive-upload-cutoff=16384k sync
 
 download
 rclone --transfers=12  copy
