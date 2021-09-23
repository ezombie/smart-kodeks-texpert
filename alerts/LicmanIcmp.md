# LicmanIcmp

Описание
---
Проверка на доступность удалённого сервера командой **Ping** (протокол ICMP).

Что проверяется
---
Проверяется что удалённый сервер доступен в сети интернет. В норме показывает,
что операционная система на удалённом сервере работоспособна.

Нормальное состояние
---

Команда ping <имя хоста> завершается успешно.
```shell
ping smart.uniclass.ru
PING smart.uniclass.ru (217.23.83.5) 56(84) bytes of data.
64 bytes from proxy.uniclass.ru (217.23.83.5): icmp_seq=1 ttl=56 time=33.0 ms
....
64 bytes from proxy.uniclass.ru (217.23.83.5): icmp_seq=3 ttl=56 time=33.0 ms
```


Аварийное состояние
---

Команда ping <имя хоста> сообщеает что удалённых хост недоступен
```shell
ping smart.uniclass.ru
PING smart.uniclass.ru (217.23.83.5) 56(84) bytes of data.
From smart.uniclass.ru icmp_seq=1 Destination Host Unreachable
```

Причины
---

- удалённый сервер не доступен через сеть интернет
- сервер выключен
- firewall блокирует трафик со стороны 'smart.uniclass.ru' по протоколу ICMP

Устранение
---

- правильно настроить сервер
- включить сервер
- настроить firewall для пропуска трафика со стороный 'smart.uniclass.ru'
