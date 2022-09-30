# script_info
#!/bin/bash
user_id=`cat /etc/passwd | grep $1 | awk -F: `{ print $1,$3,$4,$6,$7 }'`
echo "$user_id `id $1 | cut -d " " -f 3`"
