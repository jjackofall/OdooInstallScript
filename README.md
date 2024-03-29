# OdooInstallScript

limit-memory-soft = workers * 640MB
limit-memory-hard = workers * 768MB

### 640 & 768 MB are default values per single worker

limit-memory-soft - 4 * 640 * 1024 * 1024

## Worker number calculation
### Rule of thumb : (#CPU * 2) + 1

Cron workers need CPU
1 worker ~= 6 concurrent users

```
limit_memory_hard = 1610612736
limit_memory_soft = 629145600
limit_request = 8192
limit_time_cpu = 600
limit_time_real = 1200
max_cron_threads = 1
workers = 2
```

# [Wkhtmltopdf](https://wkhtmltopdf.org/ "Wkhtmltopdf's Homepage") Install Script

Wkhtmltopdf Script for Ubuntu

## Installation procedure

##### 1. Download the script:
```
sudo wget https://raw.githubusercontent.com/jjackofall/OdooInstallScript/main/wkhtmltopdf_install.sh
```

#### 2. Make the script executable
```
sudo chmod +x wkhtmltopdf_install.sh
```
##### 4. Execute the script:
```
sudo ./wkhtmltopdf_install.sh
```
