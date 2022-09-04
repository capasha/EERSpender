# EESpender / EERSpender
A tool that automatically collects login rewards, and spends energy on the newest items in the Energy Shop.

EESpender is created by Atillabyte. The project can be found here: [https://github.com/atillabyte/EESpender](https://github.com/atillabyte/EESpender)  
EESpender have been changed to work for EER.  

# Using EESpender

All that is necessary is running the process with proper account parameters.  
You could also make a file named **accounts.dat** whith **email password** inside.  

This can be done with Cron (Linux), or Task Scheduler (Windows).

# Examples
## crontab
```shell
0 */2 * * * cd /home/root/eespender/ && mono EESpender.exe "user@example.com" "password" 2>&1 & 
```

## crontab (multiple accounts)
```shell
0 */2 * * * cd /home/root/eespender/ && mono EESpender.exe "user1@example.com" "password" "user2@example.com" "password2" 2>&1 & 
```
