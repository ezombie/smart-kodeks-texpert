## Как это устроено?

Сервис «СМАРТ-мониторинг» (здесь и далее – СМАРТ) создан для автоматизированного контроля и последующей аналитики качества, технического состояния внедренных у клиентов информационно-справочных систем Кодекс/Техэксперт (здесь и далее – ИСС, установки, объекты). 
СМАРТ обладает аналитическими и статистическими функциями, по результатам от которых дистрибьютор-пользователь СМАРТа в кратчайшие сроки может делать максимально объективные выводы о качестве, количестве и частоте использования внедренных у своих клиентов ИСС и использовать полученную информацию с целью повышения качества сбыта и сопровождения ИСС и увеличения финансовых и других показателей своего предприятия-дистрибьютора.

Условно СМАРТ можно разделить на четыре части – 
- Система автоматизированного сбора статистических данных (здесь и далее — отчетов sysinfo) с подконтрольных СМАРТу объектов; 
- Система оповещений; 
- Система графической интерпретации собранных данных;
- Система автоматизации.

Для целей данного руководства применяются следующие специфические термины: 
- Система оповещений именуется Алертингом, ее элементы именуются алертами;
- Система графической интерпретации собранных отчетов sysinfo именуется Grafana (он же - Личный Кабинет пользователя СМАРТа), элементы Grafana именуются дашбордами, элементы дашборда - графики и таблицы в этих дашбордах;
- пользователь СМАРТа – пользователь-дистрибьютор ИСС, предоставивший набор объектов, которые он желает отслеживать с помощью СМАРТа.

Для функционирования Системы сбора отчетов sysinfo необходимо предоставить разработчику СМАРТа список объектов, которые требуется отслеживать. 
В некоторых случаях достаточно адреса в сети интернет для этого (URL), в других случаях - внедрить на установке ИСС у клиента небольшой скриптовый файл (здесь и далее - smartupload) и настроить его регулярное автоматическое исполнение средствами ОС. 

На момент написания данного руководства СМАРТ осуществляет свои функции со следующими типами контролируемых объектов: 
- клиенты-пользователи ИСС, чьи комплекты внедрены на компьютерных мощностях самих клиентов и имеют выход в интернет: в этом случае у клиента-пользователя рядом с установкой внедряется smartupload и настраивается его регулярное исполнение с помощью соответствующего функционала ОС, в которой существует сама установка (см. Руководство по внедрению СМАРТа);
- клиенты-пользователи ИСС, чьи комплекты внедрены на компьютерных мощностях самих клиентов и не имеют выхода в интернет (так же именуемый как «закрытый контур»): в этом случае у клиента-пользователя рядом с установкой внедряется smartupload и настраивается его регулярное исполнение с помощью соответствующего функционала ОС, в которой существует сама установка. 
**НЮАНС:** в этом случае отправка сохраненного отчета sysinfo выполняется вручную силами пользователя СМАРТа (см. Руководство по внедрению СМАРТа);
- клиенты-пользователи ИСС, чьи комплекты внедрены на сторонних компьютерных мощностях (с использованием облачных технологий, в том числе с использованием сервиса «Техэксперт.Облако») и имеют выход в интернет: в этом случае могут быть нюансы внедрения smartupload, кои оговариваются индивидуально с разработчиком СМАРТа (см. Руководство по внедрению СМАРТа);
- клиенты-пользователи ИСС, кто использует простые онлайн-доступы к ИСС, развернутые на компьютерных мощностях правообладателя ИСС (он же - ДЦ, Дистрибьюторский Центр): в этом случае на мониторинг предоставляется список web-адрес (URL), логины и пароли по каждому адресу, такие же, какие выдаются клиенту-пользователю ИСС. Шаблон списка можно (и нужно) получить у разработчика СМАРТа.

Обращаем внимание, что на ВСЕХ типах контролируемых объектов СМАРТ НЕ занимает рабочие места (лицензии), ограниченное количество которых прописано в reg-файле на установке, равно как НЕ использует единицы биллинга, если речь идет о контроле простых онлайн-доступов.
Для получения результатов работы Алертинга пользователю СМАРТа необходимо предоставить разработчику СМАРТа адрес электронной почты (личная или корпоративная) и/или работающий аккаунт в Telegram куда будут приходить алерты.

Для оценки результатов работы Grafana и для оценки результатов работы Системы автоматизации пользователю необходимо любое устройство, имеющее выход в интернет и установленный на нем браузер крайних стабильных версий. 
Пользователю заводится Личный кабинет (или несколько, в зависимости от того какое количество пользователей СМАРТа должны иметь доступ к результатам деятельности СМАРТа), где отображаются все зарегистрированные в СМАРТе клиенты-пользователи ИСС, закрепленные за данным менеджером пользователя-дистрибьютора.

Примечание: полные инструкции по внедрению и настройке СМАРТа у клиентов-пользователей ИСС следует изучать в соответствующих Руководствах. 
Их можно получить у разработчика СМАРТа. 
Кроме того, в случае затруднений всегда можно проконсультироваться с самим разработчиком СМАРТа в телеграмм-чате «СМАРТ-мониторинга» - https://t.me/+uRkrNE_SNYY0YTUy , а также в индивидуальных телеграмм-чатах, которые заводятся по факту постановки объектов на контроль СМАРТом: один такой чат для работы Алертинга обязателен, второй – для индивидуальных консультаций.

[Читай дальше](020-auto-collect-sysinfo.md)

[Вернуться к Оглавлению](Readme.md)