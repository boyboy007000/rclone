# rclone
#intall
curl https://rclone.org/install.sh | sudo bash

upload or sync with large file
 rclone --transfers=32 --checkers=16 --drive-chunk-size=16384k --drive-upload-cutoff=16384k --stats-log-level NOTICE   -vvv  sync
 #upload or sync with large file with symlinks
  rclone --transfers=32 --checkers=16 --drive-chunk-size=16384k --drive-upload-cutoff=16384k --stats-log-level NOTICE   -vvv  -L sync
 
 download
 rclone --transfers=12  --stats-log-level NOTICE   -vvv copy 

--drive-root-folder-id

Delete file in folder
rclone delete epu:rclone/ --drive-use-trash=false --min-size=1B

delete folder

rclone purge epu:rclone/ --drive-use-trash=false --min-size=1B
