# adblock_keenetic
Автоматическая установка для выборочного обхода блокировок на маршрутизаторах с прошивкой Keenetic OS.(Entware)

Загрузите скрипт установки:

opkg install wget ca-certificates
wget --no-check-certificate -O /opt/bin/unblock_keenetic.sh https://raw.githubusercontent.com/alexku44/adblock_keenetic/master/unblock_keenetic.sh
chmod +x /opt/bin/unblock_keenetic.sh
Установка (автоматическое выполнение шагов 1-12):

unblock_keenetic.sh
После автоматической перезагрузки маршрутизатора для реализации «Дополнительный обход фильтрации DNS-запросов провайдером» (если вам это нужно) выполните команду:

unblock_keenetic.sh dnscrypt
Удаление обхода блокировок:

unblock_keenetic.sh remove
Аналогичный скрипт для Padavan. ВНИМАНИЕ! Скрипт пока тоже не проверялся на реальном устройстве. Только для экспериментаторов. Все остальные должны использовать ручной метод установки, описанный в статье.

Загрузка скрипта:

opkg install wget ca-certificates
wget --no-check-certificate -O /opt/bin/unblock_padavan.sh https://raw.githubusercontent.com/alexku44/adblock_keenetic/master/padavan/unblock_padavan.sh
chmod +x /opt/bin/unblock_padavan.sh
