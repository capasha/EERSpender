# EESpender / EERSpender
A tool that automatically collects login rewards, and spends energy on the newest items in the Energy Shop.

EESpender is created by Atillabyte. The project can be found here: [https://github.com/atillabyte/EESpender](https://github.com/atillabyte/EESpender)  
EESpender have been changed to work for EER.  

# Using EESpender

All that is necessary is running the process with proper account parameters.  
You could also make a file named **accounts.dat** whith **email password** inside.  

This can be done with Cron (Linux), or Task Scheduler (Windows).

# Examples
## crontab (Linux)
```shell
0 */2 * * * cd /home/root/eespender/ && mono EESpender.exe "user@example.com" "password" 2>&1 & 
```

## crontab (multiple accounts) (Linux)
```shell
0 */2 * * * cd /home/root/eespender/ && mono EESpender.exe "user1@example.com" "password" "user2@example.com" "password2" 2>&1 & 
```

## Windows test run from commandline
```shell
EESpender.exe "user@example.com" "password"
```
Or add **user@example.com password** inside accounts.dat and click on the binary.  

## Windows Task Scheduler
Please be careful with deleting tasks you have made. So you don't delete anything accidently.  
[https://digicruncher.com/task-scheduler-in-windows-10/](https://digicruncher.com/task-scheduler-in-windows-10/)
