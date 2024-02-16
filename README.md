# Asesmen Sistem Terdistribusi

- Steven Joenior Naibaho
- Andrian Falah Kalyana
- Regi Rizaldi Nurimamsyah
- Rizki Febryano

Lampiran konfigurasi replika (mysql.conf):

master to master:

Server A master:
bind-address = 192.168.163.159
server-id = 1
log_bin = /var/log/mysql/mysql-bin.log 

Server B master:
bind-address = 192.168.163.160
server-id = 2
log_bin = /var/log/mysql/mysql-bin.log 

Master to slave:

Server A master
bind-address = 192.168.163.159
server-id = 1
log_bin = /var/log/mysql/mysql-bin.log 

Server C slave:
bind-address = 192.168.163.161
server-id = 3
log_bin = /var/log/mysql/mysql-bin.log 
