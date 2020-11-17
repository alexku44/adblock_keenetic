Автоматическая установка для выборочного обхода блокировок на маршрутизаторах с прошивкой Keenetic OS.(entware)


Загрузите скрипт установки:
```bash
opkg install wget ca-certificates
wget --no-check-certificate -O /opt/bin/unblock_keenetic.sh https://raw.githubusercontent.com/alexku44/adblock_keenetic/blob/main/unblock_keenetic.sh
chmod +x /opt/bin/unblock_keenetic.sh
```

Установка (автоматическое выполнение шагов 1-12):
```bash
unblock_keenetic.sh
```

После автоматической перезагрузки маршрутизатора для реализации «Дополнительный обход фильтрации DNS-запросов провайдером» (если вам это нужно) выполните команду:
```bash
unblock_keenetic.sh dnscrypt
```

Удаление обхода блокировок:
```bash
unblock_keenetic.sh remove
```
