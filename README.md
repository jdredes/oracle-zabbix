# Zabbix Oracle Template

Created by Josué Pirolo 04/2016

Step 1 - Create a directory to store the script and config files generated by the script

<b>mkdir -p /var/lib/zabbix/scripts/<br>
chown -R oracle:dba /var/lib/zabbix/scripts/</b>
<br>
Step 2 - execute <b>git clone https://github.com/crmall/oracle-zabbix.git</b><br>
cd oracle-zabbix/
<br>
Step 3 - Execute <b>sh zabbix_info.sh oracle_env</b><br>
Informe o usuario SYSADMIN<br>
<b>system</b><br>
Informe a senha do usuario SYSADMIN<br>
<b>*******</b><br>
It will create the user zabbix and set the needs GRANTS and set de ORACLE_HOME paths.
<br>
Step 4 - Now, log in with root user and do the following:<br>
<b> cat zabbix_agentd_conf >> /etc/zabbix/zabbix_agentd.conf</b><br>
Restart the zabbix-agent service and configure de Host in zabbix server interface.

