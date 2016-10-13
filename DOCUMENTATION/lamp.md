# XAMP for LINUX

----

### lamp lancer
sudo /opt/lampp/lampp start
sudo /opt/lampp/manager-linux-x64.run

###vérifier les APACHE et SQL lancés
ps aux | grep apache2  
ps aux | grep mysql

###arrêter tout apache
### return Stopping apache2 (via systemctl): apache2.service.
sudo /etc/init.d/apache2 stop
sudo /opt/lampp/manager-linux-x64.run stop
sudo /opt/lampp/lampp stop

### HARD STOP mysql
sudo /etc/init.d/mysql stop                                                                  
[sudo] Mot de passe de vmllmv :
[ ok ] Stopping mysql (via systemctl): mysql.service.

----

## ZSHRC / BACHRC alias
avant de lancer mon lampp faur un HARD STOP
```shell
$ lamppinit
```
lancer ou un redémarage des services
```shell
$ lamppstart
$ lampprestart
```
arrêter
```shell
$ lamppstop
```