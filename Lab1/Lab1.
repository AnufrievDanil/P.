# Получение сведений о системе

## Цель работы

Получить сведения об используемой системе

## Исходные данные

1. Стационарный ПК собранный на коленке

2. Kali GNU/Linux Rolling

3. Терминал: QTerminal 1.2.0

## План

1. Ввод команд в эмулятор терминала

2. Анализ данных

## Ход работы

1. Для начала получим сведения об используемом дистрибутиве:

```
┌──(root㉿kali)-[/home/kali]
└─# lsb_release -a
No LSB modules are available.
Distributor ID: Kali
Description:    Kali GNU/Linux Rolling
Release:        2023.1
Codename:       kali-rolling
```

В результате выполнения данной команды было определён используемый дистрибутив - Kali GNU/Linux Rolling

2.Затем получим сведения о версии ядра:

```
┌──(root㉿kali)-[/home/kali]
└─# uname -a
Linux kali 6.1.0-kali5-amd64 #1 SMP PREEMPT_DYNAMIC Debian 6.1.12-1kali2 (2023-02-23) x86_64 GNU/Linux
```

В результате выполнения данной команды была получена версия ядра - 6.1.0-kali5, дата компиляции ядра - 2023-02-23

3.Далее можно получить сведения о процессоре:

```
┌──(root㉿kali)-[/home/kali]
└─# cat /proc/cpuinfo | grep "model name"
model name      : Intel(R) Core(TM) i5-10600K CPU @ 4.10GHz
model name      : Intel(R) Core(TM) i5-10600K CPU @ 4.10GHz
model name      : Intel(R) Core(TM) i5-10600K CPU @ 4.10GHz
model name      : Intel(R) Core(TM) i5-10600K CPU @ 4.10GHz
```

Было определено, что используемый процессор - четырёъпоточный Intel(R) Core(TM) i5-10600K с тактовой частотой 4.10GHz.

4.Далее получим последние 30 строк логов системы:

```
┌──(root㉿kali)-[/home/kali]
└─# journalctl -q -b| tail -n 30
May 20 09:56:27 kali systemd[1]: user-runtime-dir@111.service: Deactivated successfully.
May 20 09:56:27 kali systemd[1]: Stopped user-runtime-dir@111.service - User Runtime Directory /run/user/111.
May 20 09:56:27 kali systemd[1]: Removed slice user-111.slice - User Slice of UID 111.
May 20 09:56:27 kali systemd[1]: user-111.slice: Consumed 10.036s CPU time.
May 20 09:56:28 kali systemd-networkd-wait-online[576917]: Timeout occurred while waiting for network connectivity.
May 20 09:56:28 kali apt-helper[576915]: E: Sub-process /lib/systemd/systemd-networkd-wait-online returned an error code (1)
May 20 09:56:28 kali systemd[1]: apt-daily-upgrade.service: Deactivated successfully.
May 20 09:56:28 kali systemd[1]: Finished apt-daily-upgrade.service - Daily apt upgrade and clean activities.
May 20 09:57:13 kali sudo[577656]:     kali : TTY=pts/8 ; PWD=/home/kali ; USER=root ; COMMAND=/usr/bin/su
May 20 09:57:13 kali sudo[577656]: pam_unix(sudo:session): session opened for user root(uid=0) by (uid=1000)
May 20 09:57:13 kali su[577674]: (to root) root on pts/9
May 20 09:57:13 kali su[577674]: pam_unix(su:session): session opened for user root(uid=0) by kali(uid=0)
May 20 10:00:10 kali NetworkManager[765]: <info>  [1684591210.6423] dhcp4 (eth0): state changed new lease, address=192.168.234.129
May 20 10:02:31 kali rtkit-daemon[921]: Supervising 4 threads of 2 processes of 1 users.
May 20 10:02:31 kali rtkit-daemon[921]: Supervising 4 threads of 2 processes of 1 users.
May 20 10:02:33 kali rtkit-daemon[921]: Supervising 4 threads of 2 processes of 1 users.
May 20 10:02:33 kali rtkit-daemon[921]: Supervising 4 threads of 2 processes of 1 users.
May 20 10:02:33 kali rtkit-daemon[921]: Supervising 4 threads of 2 processes of 1 users.
May 20 10:02:33 kali rtkit-daemon[921]: Supervising 4 threads of 2 processes of 1 users.
May 20 10:02:33 kali rtkit-daemon[921]: Supervising 4 threads of 2 processes of 1 users.
May 20 10:02:33 kali rtkit-daemon[921]: Supervising 4 threads of 2 processes of 1 users.
May 20 10:05:01 kali CRON[581651]: pam_unix(cron:session): session opened for user root(uid=0) by (uid=0)
May 20 10:05:01 kali CRON[581652]: (root) CMD (command -v debian-sa1 > /dev/null && debian-sa1 1 1)
May 20 10:05:01 kali CRON[581651]: pam_unix(cron:session): session closed for user root
May 20 10:09:01 kali CRON[583587]: pam_unix(cron:session): session opened for user root(uid=0) by (uid=0)
May 20 10:09:01 kali CRON[583588]: (root) CMD (  [ -x /usr/lib/php/sessionclean ] && if [ ! -d /run/systemd/system ]; then /usr/lib/php/sessionclean; fi)
May 20 10:09:01 kali CRON[583587]: pam_unix(cron:session): session closed for user root
May 20 10:09:20 kali systemd[1]: Starting phpsessionclean.service - Clean php session files...
May 20 10:09:20 kali systemd[1]: phpsessionclean.service: Deactivated successfully.
May 20 10:09:20 kali systemd[1]: Finished phpsessionclean.service - Clean php session files.
```

## Оценка результата

В результате лабораторной работы была получена базовая информация об используемой системе.

## Вывод

Таким образом. мы научились, используя команды Linux, получать сведения о системе.
