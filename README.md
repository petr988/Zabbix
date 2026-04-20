Домашнее задание к занятию "Название занятия" - Фамилия и имя студента
Инструкция по выполнению домашнего задания
Сделайте fork данного репозитория к себе в Github и переименуйте его по названию или номеру занятия, например, https://github.com/имя-вашего-репозитория/git-hw или https://github.com/имя-вашего-репозитория/7-1-ansible-hw).
Выполните клонирование данного репозитория к себе на ПК с помощью команды git clone.
Выполните домашнее задание и заполните у себя локально этот файл README.md:
впишите вверху название занятия и вашу фамилию и имя
в каждом задании добавьте решение в требуемом виде (текст/код/скриншоты/ссылка)
для корректного добавления скриншотов воспользуйтесь инструкцией "Как вставить скриншот в шаблон с решением
при оформлении используйте возможности языка разметки md (коротко об этом можно посмотреть в инструкции по MarkDown)
После завершения работы над домашним заданием сделайте коммит (git commit -m "comment") и отправьте его на Github (git push origin);
Для проверки домашнего задания преподавателем в личном кабинете прикрепите и отправьте ссылку на решение в виде md-файла в вашем Github.
Любые вопросы по выполнению заданий спрашивайте в чате учебной группы и/или в разделе “Вопросы по заданию” в личном кабинете.
Желаем успехов в выполнении домашнего задания!

Дополнительные материалы, которые могут быть полезны для выполнения задания
Руководство по оформлению Markdown файлов
Задание 1
apt install postgres
    4  apt install postgressql
    5  apt install postgresql
    6  wget https://repo.zabbix.com/zabbix/7.0/ubuntu/pool/main/z/zabbix-release/zabbix-release_latest_7.0+ubuntu24.04_all.deb
    7  ls
    8  dkpg -i zabbix-release_latest_7.0+ubuntu24.04_all.deb
    9  dpkg -i zabbix-release_latest_7.0+ubuntu24.04_all.deb
   10  ls -la /etc/apt/sources.list.d/
   11  cat /etc/apt/sources.list.d/zabbix.list 
   12  apt update
   13  apt install zabbix-server-pgsql zabbix-frontend-php php8.3-pgsql zabbix-apache-conf zabbix-sql-scripts
   14  systemctl status zabbix-server.service 
   15  su - postgres -c 'psql' --command "CREATE USER zabbix WITH PASSWORD '\'123456789\'';"'
   16  u -
   17  su -
   18  exit
   19  su petr
   20  su - postgres -c "psql -c \"CREATE USER zabbix WITH PASSWORD '123456789';\""
   21  sudo -u postgres createdb -O zabbix zabbix 
   22  zcat /usr/share/zabbix-sql-scripts/postgresql/server.sql.gz | sudo -u zabbix psql zabbix 
   23  fine / -name zabbix_agentd
   24  find / -name zabbix_agentd
   25  sudo find / -name zabbix_agentd
   26  cd /etc
   27  cd /zabbix
   28  ll
   29  cd zabbix
   30  ll
   31  nano zabbix_server.conf 
   32  systamctl restart zabbix-server appache2
<img width="1512" height="877" alt="image" src="https://github.com/user-attachments/assets/4bf72232-7c7b-4340-b1ce-d58c0987b5a0" />



....
....
....
....
При необходимости прикрепитe сюда скриншоты ![Название скриншота 1](ссылка на скриншот 1)

Задание 2
dpkg -i zabbix-release_latest_7.0+ubuntu24.04_all.deb
   56  apt update 
   57  apt install zabbix-agent
   58  systemctl status zabbix-agent.servuce
   59  systemctl status zabbix-agent.service
   60  find / -name zabbix_agentd.conf
   61  nano /etc/zabbix/zabbix_agentd.conf
   62  sytemctl restart zabbix_agent.service
   63  systemctl restart zabbix_agent.service
   64  systemctl restart zabbix-agent.service
<img width="1187" height="721" alt="image" src="https://github.com/user-attachments/assets/47e7f61f-a730-4cb3-b30e-bb33eab909fc" />
