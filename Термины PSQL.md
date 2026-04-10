
[[PSQL]]
ACID
Atomicity ([](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-ATOMICITY)_[Атомарность](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-ATOMICITY "Атомарность")_), Consistency ([](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-CONSISTENCY)_[Согласованность](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-CONSISTENCY "Согласованность")_), Isolation ([](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-ISOLATION)_[Изолированность](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-ISOLATION "Изолированность")_) и Durability ([](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DURABILITY)_[Надёжность](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DURABILITY "Надёжность")_). Этот набор свойств транзакций в базе данных должен гарантировать корректность операций при параллельном выполнении, а также в случае ошибок, при отключении питания и т. п.

DELETE
SQL-команда, которая удаляет [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TUPLE)_[строки](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TUPLE "Кортеж")_ из данной [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE)_[таблицы](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE "Таблица")_ или [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION)_[отношения](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION "Отношение")_.
Подробности в описании [DELETE](https://postgrespro.ru/docs/postgresql/current/sql-delete.html "DELETE").

GMT
См. [UTC](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-UTC).

GRANT
SQL-команда, дающая [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-USER)_[пользователю](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-USER "Пользователь")_ или [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-ROLE)_[роли](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-ROLE "Роль")_ доступ к определённым объектам в [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE)_[базе данных](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE "База данных")_.
Подробности в описании [GRANT](https://postgrespro.ru/docs/postgresql/current/sql-grant.html "GRANT").

INSERT
SQL-команда, добавляющая в [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE)_[таблицу](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE "Таблица")_ новые данные.
Поробности в описании [INSERT](https://postgrespro.ru/docs/postgresql/current/sql-insert.html "INSERT").

LSN
См. [Последовательный номер в журнале](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-LOG-SEQUENCE-NUMBER).

MERGE
Команда SQL для добавления, изменения или удаления [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TUPLE)_[строк](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TUPLE "Кортеж")_ с определёнными условиями в заданной [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE)_[таблице](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE "Таблица")_ с использованием данных из исходного [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION)_[отношения](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION "Отношение")_

Подробности в описании [MERGE](https://postgrespro.ru/docs/postgresql/current/sql-merge.html "MERGE").

NULL
Понятие неопределённости, выражаемой как NULL, является ключевым в теории реляционных баз данных. Оно обозначает отсутствие какого-либо определённого значения.

REVOKE
Команда, лишающая указанные [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-ROLE)_[роли](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-ROLE "Роль")_ доступа к определённому набору объектов [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE)_[базы данных](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE "База данных")_.
Подробности в описании [REVOKE](https://postgrespro.ru/docs/postgresql/current/sql-revoke.html "REVOKE").

ROLLBACK
Команда, отменяющая все операции, выполненные с начала [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TRANSACTION)_[транзакции](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TRANSACTION "Транзакция")_.
Подробности в описании [ROLLBACK](https://postgrespro.ru/docs/postgresql/current/sql-rollback.html "ROLLBACK").

SELECT
SQL-команда, позволяющая запросить данные из [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE)_[базы](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE "База данных")_. Обычно команды `SELECT` не должны изменять состояние [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE)_[базы](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE "База данных")_ никаким образом, однако выполняемые ими запросы могут вызывать [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-FUNCTION)_[функции](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-FUNCTION "Функция (подпрограмма)")_, в качестве побочного эффекта меняющие данные.
Подробности в описании [SELECT](https://postgrespro.ru/docs/postgresql/current/sql-select.html "SELECT").

SQL-объект
Любой объект, который может быть создан командой `CREATE`. Большинство объектов относятся к одной базе данных, поэтому они обычно называются _локальными объектами_.

TOAST
Механизм, который обеспечивает хранение больших атрибутов строк таблицы, размещая их в дополнительной _TOAST-таблице_. У каждого отношения с большими атрибутами имеется собственная TOAST-таблица.
Подробности в [Разделе 66.2](https://postgrespro.ru/docs/postgresql/current/storage-toast.html "66.2. TOAST").

UPDATE
SQL-команда, вносящая изменения в уже существующие [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TUPLE)_[строки](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TUPLE "Кортеж")_ определённой [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE)_[таблицы](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE "Таблица")_. Эта команда не добавляет и не удаляет строки.
Подробности в описании [UPDATE](https://postgrespro.ru/docs/postgresql/current/sql-update.html "UPDATE").

UTC
Всемирное координированное время (UTC) — основная глобальная система отсчёта времени, близкая к времени нулевого меридиана. Часто ошибочно называют средним временем по Гринвичу (GMT).

WAL
См. [Журнал предзаписи](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL).

Автоочистка (autovacuum)
Набор фоновых процессов, регулярно выполняющих операции [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-VACUUM)_[очистки](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-VACUUM "Очистка (VACUUM)")_ и [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-ANALYZE)_[анализа](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-ANALYZE "Анализ (операция)")_. [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-AUXILIARY-PROC)_[Вспомогательный процесс](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-AUXILIARY-PROC "Вспомогательный процесс")_, который координирует работу и существует всегда (если не отключена автоочистка), называется «autovacuum launcher» (_процесс запуска автоочистки_), а каждый процесс, который запускается для выполнения задач, называется «autovacuum worker» (_рабочий процесс автоочистки_).
Подробности в [Подразделе 24.1.6](https://postgrespro.ru/docs/postgresql/current/routine-vacuuming#AUTOVACUUM "24.1.6. Демон автоочистки").

Агрегатная функция (подпрограмма)
[](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-FUNCTION)_[Функция](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-FUNCTION "Функция (подпрограмма)")_, которая сводит к одному значению (_агрегирует_) множество входных значений, например, подсчитывая их количество, складывая их или вычисляя среднее.
Подробности в [Разделе 9.21](https://postgrespro.ru/docs/postgresql/current/functions-aggregate.html "9.21. Агрегатные функции").
См. также [Оконная функция (подпрограмма)](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WINDOW-FUNCTION).

Анализ (операция)
Сбор статистики по данным в [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE)_[таблицах](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE "Таблица")_ и других [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION)_[отношениях](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION "Отношение")_, помогающий [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-PLANNER)_[планировщику запросов](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-PLANNER "Планировщик запросов")_ находить оптимальные способы выполнения [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-QUERY)_[запросов](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-QUERY "Запрос")_.
(Не путайте этот термин с указанием `ANALYZE` команды [EXPLAIN](https://postgrespro.ru/docs/postgresql/current/sql-explain.html "EXPLAIN").)
Подробности в [ANALYZE](https://postgrespro.ru/docs/postgresql/current/sql-analyze.html "ANALYZE").

Аналитическая функция
См. [Оконная функция (подпрограмма)](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WINDOW-FUNCTION).

Асинхронный I/O (AIO)
Асинхронный ввод-вывод (AIO) означает неблокирующее (асинхронное) выполнение операций ввода-вывода, в отличие от синхронного ввода-вывода, где процесс блокируется на всё время выполнения таких операций.
При AIO запуск операции ввода-вывода и ожидание её результата отделены друг от друга, что позволяет запускать несколько операций ввода-вывода параллельно, а также параллельно с такими операциями выполнять задачи с высокой нагрузкой на процессор. Однако возможность параллельного выполнения операций достигается ценой усложнения реализации.
См. также [Ввод-вывод](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-IO).

Атомарность
Свойство [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TRANSACTION)_[транзакции](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TRANSACTION "Транзакция")_, которое заключается в том, что в результате транзакции все её операции выполняются вместе, либо не выполняются совсем. Кроме того, частичные изменения исключены в случае сбоя системы в процессе выполнения транзакции. Это одно из свойств ACID.

Атомарный
Применительно к [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATUM)_[данным](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATUM "Элемент данных")_ означает, что элемент данных нельзя разделить на меньшие части.
Применительно к [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TRANSACTION)_[транзакциям в базах данных](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TRANSACTION "Транзакция")_ см. [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-ATOMICITY)_[атомарность](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-ATOMICITY "Атомарность")_.

Атрибут
Элемент с определённым именем и типом данных, содержащийся в [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TUPLE)_[кортеже](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TUPLE "Кортеж")_.

База данных
Именованный набор [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SQL-OBJECT)_[локальных SQL-объектов](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SQL-OBJECT "SQL-объект")_.
Подробности в [Разделе 22.1](https://postgrespro.ru/docs/postgresql/current/manage-ag-overview.html "22.1. Обзор").

Базовая резервная копия
Двоичная копия всех файлов [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DB-CLUSTER)_[кластера базы данных](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DB-CLUSTER "Кластер баз данных")_, которая создаётся программой [pg_basebackup](https://postgrespro.ru/docs/postgresql/current/app-pgbasebackup.html "pg_basebackup"). При наличии файлов WAL эту копию можно использовать в качестве отправной точки для восстановления, трансляции журналов или потоковой репликации.

Блокировка
Механизм, позволяющий некоторому процессу ограничивать или запрещать параллельный доступ к ресурсу.

Ввод-вывод (I/O)
Ввод-вывод (I/O) — это взаимодействие между программой и периферийными устройствами. В контексте СУБД ввод-вывод, как правило, означает работу с устройствами хранения данных или сетевое взаимодействие.
См. также [Асинхронный I/O](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-AIO).

Ведомый (резервный) сервер
См. [Реплика](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-REPLICA).

Ведущий (главный) сервер
См. [Ведущий (сервер)](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-PRIMARY-SERVER).

Ведущий (сервер)
Когда несколько [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE)_[баз данных](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE "База данных")_ связываются вместе посредством [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-REPLICATION)_[репликации](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-REPLICATION "Репликация")_, [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SERVER)_[сервер](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SERVER "Сервер")_, служащий первоисточником информации, называется _ведущим_ или _главным_.

Владелец кластера
Пользователь операционной системы, которому принадлежит [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATA-DIRECTORY)_[каталог данных](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATA-DIRECTORY "Каталог данных")_ и от имени которого запускается процесс `postgres`. Необходимо, чтобы этот пользователь существовал до создания нового [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DB-CLUSTER)_[кластера базы данных](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DB-CLUSTER "Кластер баз данных")_.
В операционных системах с пользователем `root` указанному пользователю запрещается быть владельцем кластера.

Внешний ключ
Вид [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-CONSTRAINT)_[ограничения](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-CONSTRAINT "Ограничение")_, определяемый для одного или нескольких [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-COLUMN)_[столбцов](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-COLUMN "Столбец")_ в [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE)_[таблице](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE "Таблица")_ и требующий, чтобы значения в этих [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-COLUMN)_[столбцах](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-COLUMN "Столбец")_ указывали на ноль или одну [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TUPLE)_[строку](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TUPLE "Кортеж")_ в другой (в редких случаях, той же) [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE)_[таблице](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE "Таблица")_.

Временная таблица
[](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE)_[Таблица](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE "Таблица")_, существующая либо в рамках [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SESSION)_[сеанса](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SESSION "Сеанс")_, либо в рамках [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TRANSACTION)_[транзакции](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TRANSACTION "Транзакция")_, в соответствии с выбранным при её создании режимом. Такие таблицы не являются [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-LOGGED)_[журналируемыми](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-LOGGED "Журналируемое отношение")_, и их содержимое не видно в других сеансах. Временные таблицы часто применяются, когда нужно сохранить промежуточные результаты в ходе сложной операции.
Подробности в описании [CREATE TABLE](https://postgrespro.ru/docs/postgresql/current/sql-createtable.html "CREATE TABLE").

Вспомогательный процесс
Процесс, относящийся к [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-INSTANCE)_[экземпляру](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-INSTANCE "Экземпляр СУБД")_ СУБД и отвечающий за определённую фоновую задачу для этого экземпляра. К числу вспомогательных процессов относятся [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-AUTOVACUUM)_[процесс запуска автоочистки](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-AUTOVACUUM "Автоочистка (autovacuum)")_ (но не рабочие процессы автоочистки), [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-BACKGROUND-WRITER)_[процесс фоновой записи](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-BACKGROUND-WRITER "Процесс фоновой записи")_, [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-CHECKPOINTER)_[процесс контрольных точек](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-CHECKPOINTER "Процесс контрольных точек (checkpointer)")_, [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-LOGGER)_[процесс протоколирования](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-LOGGER "Процесс протоколирования")_, [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-STARTUP-PROCESS)_[процесс запуска](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-STARTUP-PROCESS "Процесс запуска")_, [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL-ARCHIVER)_[процесс архивации WAL](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL-ARCHIVER "Процесс архивации WAL")_, [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL-RECEIVER)_[процесс-приёмник WAL](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL-RECEIVER "Процесс-приёмник WAL")_ (но не [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL-SENDER)_[процессы-передатчики WAL](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL-SENDER "Процесс-передатчик WAL")_), [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL-SUMMARIZER)_[процесс создания сводок WAL](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL-SUMMARIZER "Процесс создания сводок WAL")_ и [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL-WRITER)_[процесс записи WAL](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL-WRITER "Процесс записи WAL")_.

Домен
Пользовательский тип данных, основанный на другом нижележащем типе данных. Он действует так же, как нижележащий тип, за исключением возможного ограничения набора допустимых значений.
Подробности в [Разделе 8.18](https://postgrespro.ru/docs/postgresql/current/domains.html "8.18. Типы доменов").

Журнал предзаписи
Журнал, в котором отслеживаются изменения в [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DB-CLUSTER)_[кластере баз данных](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DB-CLUSTER "Кластер баз данных")_, производимые при выполнении операций пользователями и самой системой. Он содержит множество отдельных [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL-RECORD)_[записей WAL](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL-RECORD "Запись WAL")_, вносимых последовательно в [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL-FILE)_[файлы WAL](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL-FILE "Файл WAL")_.

Журналируемое отношение
[](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE)_[Таблица](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE "Таблица")_ считается [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-LOGGED)_[журналируемой](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-LOGGED "Журналируемое отношение")_, если вносимые в неё изменения проходят через [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL)_[WAL](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL "Журнал предзаписи")_. По умолчанию все обычные таблицы являются журналируемыми. Таблицу можно сделать [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-UNLOGGED)_[нежурналируемой](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-UNLOGGED "Нежурналируемое отношение")_ либо во время создания, либо выполнив команду `ALTER TABLE`.
Запись
См. [Кортеж](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TUPLE).

Запись WAL
Низкоуровневое описание отдельного изменения данных. Оно содержит достаточно информации для воспроизведения (_повторного применения_) этого изменения в случае сбоя системы до переноса изменения в базу. В записях WAL используется непечатаемый двоичный формат.
Подробности в [Разделе 28.6](https://postgrespro.ru/docs/postgresql/current/wal-internals.html "28.6. Внутреннее устройство WAL").

Запись журнала
Устаревшее название [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL-RECORD)_[записи WAL](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL-RECORD "Запись WAL")_.

Запрос
Указание, передаваемое клиентом [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-BACKEND)_[обслуживающему процессу](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-BACKEND "Обслуживающий процесс (backend)")_, в результате выполнения которого меняются данные в базе или выдаются результаты для клиента.

Идентификатор транзакции
Числовой уникальный идентификатор, последовательно назначаемый каждой транзакции при первой операции, меняющей данные. Часто он сокращённо обозначается _xid_. Когда эти идентификаторы хранятся на диске, каждый занимает всего 32 бита, поэтому только около 4 миллиардов пишущих транзакций могут получить уникальные идентификаторы. Чтобы система баз данных могла работать дольше, дополнительно используется _эпоха_, которая также имеет размер 32 бита. Когда счётчик транзакций достигает максимально возможного значения, он сбрасывается до `3` (меньшие значения зарезервированы) и значение эпохи увеличивается на 1. В некоторых контекстах значения эпохи и xid рассматриваются вместе как одна 64-битная величина; за подробностями обратитесь к [Разделу 67.1](https://postgrespro.ru/docs/postgresql/current/transaction-id.html "67.1. Транзакции и идентификаторы").
Подробности в [Разделе 8.19](https://postgrespro.ru/docs/postgresql/current/datatype-oid.html "8.19. Идентификаторы объектов").

Изолированность
Свойство, которое заключается в том, что результаты транзакции не видны для [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-CONCURRENCY)_[параллельных транзакций](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-CONCURRENCY "Конкурентный доступ")_, пока она не будет зафиксирована. Это одно из свойств ACID.
Подробности в [Разделе 13.2](https://postgrespro.ru/docs/postgresql/current/transaction-iso.html "13.2. Изоляция транзакций").

Индекс (отношение)
[](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION)_[Отношение](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION "Отношение")_, содержащее производную информацию от исходных данных [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE)_[таблицы](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE "Таблица")_ или [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-MATERIALIZED-VIEW)_[материализованного представления](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-MATERIALIZED-VIEW "Материализованное представление (отношение)")_. Его внутренняя структура ориентирована на быстрый поиск и извлечение исходных данных.
Подробности в описании [CREATE INDEX](https://postgrespro.ru/docs/postgresql/current/sql-createindex.html "CREATE INDEX").

Инкрементальная резервная копия
Специальная [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-BASEBACKUP)_[базовая резервная копия](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-BASEBACKUP "Базовая резервная копия")_, которая для некоторых файлов может содержать только те страницы, которые изменились с момента создания предыдущей резервной копии, а не полное содержимое каждого файла. Как и базовые резервные копии, она создаётся инструментом [pg_basebackup](https://postgrespro.ru/docs/postgresql/current/app-pgbasebackup.html "pg_basebackup").
Для восстановления инкрементальных резервных копий используется инструмент [pg_combinebackup](https://postgrespro.ru/docs/postgresql/current/app-pgcombinebackup.html "pg_combinebackup"), который объединяет инкрементальные резервные копии с базовой. После этого для приведения [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DB-CLUSTER)_[кластера базы данных](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DB-CLUSTER "Кластер баз данных")_ в согласованное состояние может использоваться [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL)_[WAL](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL "Журнал предзаписи")_.
Подробности в [Подразделе 25.3.3](https://postgrespro.ru/docs/postgresql/current/continuous-archiving#BACKUP-INCREMENTAL-BACKUP "25.3.3. Создание инкрементальной резервной копии").

Карта видимости (слой)
Хранимая структура, содержащая метаинформацию о каждой странице данных в основном слое таблицы. Для каждой страницы в ней отводится два бита: первый (`all-visible`, полностью видимая) показывает, что все кортежи в странице видны всем транзакциям, а второй (`all-frozen`, полностью замороженная) показывает, что все кортежи в странице помечены как замороженные.

Карта свободного пространства (слой)
Хранимая структура, содержащая метаинформацию о каждой странице данных в основном слое таблицы. В ней указывается, какой объём доступен для новых кортежей в каждой странице, при этом сама она специально оптимизирована для эффективного поиска свободного места для нового кортежа заданного размера.
Подробности в [Разделе 66.3](https://postgrespro.ru/docs/postgresql/current/storage-fsm.html "66.3. Карта свободного пространства").

Каталог
В стандарте SQL этот термин обозначает то, что в терминологии PostgreSQL называется [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE)_[базой данных](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE "База данных")_.
(Не путайте это понятие с понятием [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SYSTEM-CATALOG)_[системного каталога](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SYSTEM-CATALOG "Системный каталог")_).
Подробности в [Разделе 22.1](https://postgrespro.ru/docs/postgresql/current/manage-ag-overview.html "22.1. Обзор").

Каталог данных
Главный каталог [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SERVER)_[сервера](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SERVER "Сервер")_ в файловой системе, содержащий все файлы данных и подкаталоги, связанные с [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DB-CLUSTER)_[кластером баз данных](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DB-CLUSTER "Кластер баз данных")_ (за исключением [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLESPACE)_[табличных пространств](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLESPACE "Табличное пространство")_ и, возможно, [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL)_[WAL](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL "Журнал предзаписи")_). Обычно на каталог данных ссылается переменная окружения `PGDATA`.
Каталог данных в совокупности со всеми дополнительными табличными пространствами образует хранилище данных [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DB-CLUSTER)_[кластера](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DB-CLUSTER "Кластер баз данных")_.
Подробности в [Разделе 66.1](https://postgrespro.ru/docs/postgresql/current/storage-file-layout.html "66.1. Размещение файлов базы данных").

Класс (устаревшее)
См. [Отношение](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION).

Кластер баз данных
Набор баз данных и глобальных SQL-объектов, а также их общих статических и динамических метаданных. Иногда также называется просто _кластером_. Кластер баз данных создаётся с использованием программы [initdb](https://postgrespro.ru/docs/postgresql/current/app-initdb.html "initdb").
В PostgreSQL термин _кластер_ иногда обозначает также экземпляр СУБД. (Не путайте этот термин с SQL-командой `CLUSTER`.)
См. также [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-CLUSTER-OWNER)_[владелец кластера](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-CLUSTER-OWNER "Владелец кластера")_ — владелец кластера в операционной системе, и [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-BOOTSTRAP-SUPERUSER)_[начальный суперпользователь](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-BOOTSTRAP-SUPERUSER "Начальный суперпользователь")_ — владелец кластера PostgreSQL.

Кластер логической репликации
Группа, состоящая из публикующего сервера и сервера-подписчика, где публикующий сервер реплицирует изменения на подписчика.

Клиент (процесс)
Любой процесс, возможно, удалённый, который [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-CONNECTION)_[подключается](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-CONNECTION "Соединение")_ к [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-INSTANCE)_[экземпляру](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-INSTANCE "Экземпляр СУБД")_ сервера для взаимодействия с [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE)_[базой данных](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE "База данных")_ и осуществляет [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SESSION)_[сеанс](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SESSION "Сеанс")_ использования СУБД.

Ключ
Средство идентификации [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TUPLE)_[строки](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TUPLE "Кортеж")_ в [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE)_[таблице](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE "Таблица")_ или другом [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION)_[отношении](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION "Отношение")_ по значениям, содержащимся в одном или нескольких [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-ATTRIBUTE)_[атрибутах](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-ATTRIBUTE "Атрибут")_ этого отношения.

Конкурентный доступ
Концепция, определяющая возможность одновременного выполнения нескольких независимых операций в одной [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE)_[базе данных](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE "База данных")_. В PostgreSQL конкурентный доступ реализуется механизмом [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-MVCC)_[многоверсионного управления конкурентным доступом](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-MVCC "Многоверсионное управление конкурентным доступом (MVCC)")_.

Контрольная точка
Точка в последовательности записей [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL)_[WAL](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL "Журнал предзаписи")_, в которой гарантируется, что в файлы данных кучи и индекса попала вся информация из [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SHARED-MEMORY)_[общей памяти](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SHARED-MEMORY "Общая память")_, изменённая до контрольной точки; для обозначения этой точки в WAL записывается и сбрасывается _запись контрольной точки_.
Контрольной точкой также называется процедура, в ходе которой выполняются все действия, необходимые для достижения контрольной точки в приведённом выше определении. Эта процедура запускается при выполнении предопределённых условий, например по истечении заданного времени или после помещения в журнал некоторого объёма записей; также её можно вызвать командой `CHECKPOINT`.
Подробности в [Разделе 28.5](https://postgrespro.ru/docs/postgresql/current/wal-configuration.html "28.5. Настройка WAL").

Кортеж
Упорядоченный набор [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-ATTRIBUTE)_[атрибутов](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-ATTRIBUTE "Атрибут")_. Порядок атрибутов может определяться [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE)_[таблицей](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE "Таблица")_ (или другим [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION)_[отношением](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION "Отношение")_), в которой содержится кортеж. В этом случае кортеж часто называют _строкой_ таблицы. Он также может определяться структурой результирующего множества; такие кортежи иногда называют _записями_.

Куча
Содержит значения атрибутов [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TUPLE)_[строк](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TUPLE "Кортеж")_ (то есть непосредственно данные) [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION)_[отношения](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION "Отношение")_. Куча размещается в одном или нескольких [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-FILE-SEGMENT)_[файловых сегментах](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-FILE-SEGMENT "Файловый сегмент")_ в [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-FORK)_[основном слое](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-FORK "Слой")_ отношения.

Материализованное представление (отношение)
[](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION)_[Отношение](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION "Отношение")_, которое определяется оператором `SELECT` (подобно обычному [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-VIEW)_[представлению](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-VIEW "Представление")_) и при этом содержит данные как обычная [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE)_[таблица](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE "Таблица")_. Его содержимое нельзя изменить операциями `INSERT`, `UPDATE`, `DELETE` и `MERGE`.
Подробности в описании [CREATE MATERIALIZED VIEW](https://postgrespro.ru/docs/postgresql/current/sql-creatematerializedview.html "CREATE MATERIALIZED VIEW").

Материализованные данные
Свойство данных, означающее, что они были вычислены заранее и сохранены для последующего использования, а не вычисляются каждый раз «на лету».
Это используется в [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-MATERIALIZED-VIEW)_[материализованных представлениях](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-MATERIALIZED-VIEW "Материализованное представление (отношение)")_, в которых данные, полученные из запроса, определяющего представление, сохраняются на диске отдельно от первоисточника данных.
Этот термин также используется применительно к некоторым многоэтапным запросам, в которых данные, полученные на некотором этапе, сохраняются в памяти (а могут быть также вытеснены на диск), благодаря чем они могут быть многократно прочитаны на следующем этапе выполнения.

Метод доступа
Интерфейсы, которые PostgreSQL использует для доступа к данным в таблицах и индексах. Этот уровень абстракции позволяет добавлять поддержку новых типов хранения данных.
Подробности в [Главе 62](https://postgrespro.ru/docs/postgresql/current/tableam.html "Глава 62. Определение интерфейса для табличных методов доступа") и [Главе 63](https://postgrespro.ru/docs/postgresql/current/indexam.html "Глава 63. Определение интерфейса для индексных методов доступа").

Многоверсионное управление конкурентным доступом (MVCC)
Механизм, позволяющий нескольким [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TRANSACTION)_[транзакциям](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TRANSACTION "Транзакция")_ читать и записывать одни и те же строки и при этом не ждать друг друга. В PostgreSQL для реализации MVCC создаются копии (_версии_) [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TUPLE)_[кортежей](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TUPLE "Кортеж")_, когда их данные меняются; после того, как все транзакции, которым были нужны старые версии, завершаются, эти версии удаляются.

Надёжность
Гарантия того, что после [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-COMMIT)_[фиксирования](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-COMMIT "Фиксирование")_ [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TRANSACTION)_[транзакции](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TRANSACTION "Транзакция")_ произведённые ей изменения не будут потеряны даже в случае системной ошибки или краха сервера. Это одно из свойств ACID.

Начальный суперпользователь
Первый [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-USER)_[пользователь](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-USER "Пользователь")_, инициализированный в [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DB-CLUSTER)_[кластере баз данных](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DB-CLUSTER "Кластер баз данных")_.
Этот пользователь владеет всеми таблицами системного каталога в каждой базе данных. А также это роль, от имени которой автоматически выдаются все разрешения. По вышеуказанным причинам эту роль нельзя удалять.
Эта роль также ведёт себя как обычный [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE-SUPERUSER)_[суперпользователь баз данных](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE-SUPERUSER "Суперпользователь баз данных")_, и её статус суперпользователя не может быть удалён.

Нежурналируемое отношение
[](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION)_[Отношение](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION "Отношение")_, изменения в котором не отражаются в журнале [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL)_[WAL](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL "Журнал предзаписи")_. Для таких отношений отсутствует возможность репликации и восстановления после сбоя.
Нежурналируемые таблицы полезны в основном, когда требуется эффективно передать промежуточные рабочие данные между процессами.
Все [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TEMPORARY-TABLE)_[временные таблицы](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TEMPORARY-TABLE "Временная таблица")_ являются нежурналируемыми.

Область данных
См. [Каталог данных](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATA-DIRECTORY).

Обслуживающий процесс (backend)
Процесс [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-INSTANCE)_[экземпляра](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-INSTANCE "Экземпляр СУБД")_ сервера, заключающий в себе реализацию [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SESSION)_[сеанса клиента](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SESSION "Сеанс")_ и обрабатывающий его запросы.
(Не путайте это понятие с понятиями [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-BACKGROUND-WORKER)_[фоновый рабочий процесс](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-BACKGROUND-WORKER "Фоновый рабочий процесс")_ и [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-BACKGROUND-WRITER)_[фоновый процесс записи](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-BACKGROUND-WRITER "Процесс фоновой записи")_).

Общая память
Область ОЗУ, совместно используемая процессами, относящимися к одному [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-INSTANCE)_[экземпляру](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-INSTANCE "Экземпляр СУБД")_ сервера. В неё отображаются блоки файлов [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE)_[базы данных](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE "База данных")_, а также она служит временным хранилищем для [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL-RECORD)_[записей WAL](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL-RECORD "Запись WAL")_ и содержит дополнительную общую информацию. Заметьте, что общая память относится ко всему экземпляру, а не к отдельной базе данных в нём.
Самая большая часть общей памяти — _общие буферы_, в которые в виде страниц отображаются блоки файлов данных. Страница, изменённая в буфере, но ещё не сохранённая в файловой системе, называется «грязной».
Подробности в [Подразделе 19.4.1](https://postgrespro.ru/docs/postgresql/current/runtime-config-resource#RUNTIME-CONFIG-RESOURCE-MEMORY "19.4.1. Память").

Обёртка сторонних данных
Способ представления данных, находящихся не в локальной [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE)_[базе данных](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE "База данных")_, таким образом, что они отображаются как содержащиеся в локальных [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE)_[таблицах](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE "Таблица")_. Обёртка сторонних данных позволяет определить [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-FOREIGN-SERVER)_[сторонний сервер](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-FOREIGN-SERVER "Сторонний сервер")_ и [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-FOREIGN-TABLE)_[сторонние таблицы](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-FOREIGN-TABLE "Сторонняя таблица (отношение)")_.
Подробности в описании [CREATE FOREIGN DATA WRAPPER](https://postgrespro.ru/docs/postgresql/current/sql-createforeigndatawrapper.html "CREATE FOREIGN DATA WRAPPER").

Ограничение
Условие, определяющее допустимость значений данных в [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE)_[таблице](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE "Таблица")_ или атрибутов в [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DOMAIN)_[домене](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DOMAIN "Домен")_.
Подробности в [Разделе 5.5](https://postgrespro.ru/docs/postgresql/current/ddl-constraints.html "5.5. Ограничения").

Ограничение уникальности
Вид [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-CONSTRAINT)_[ограничения](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-CONSTRAINT "Ограничение")_, определённого для [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION)_[отношения](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION "Отношение")_, который ограничивает значения, допустимые в одном или нескольких столбцах таким образом, чтобы данное значение или набор значений могли присутствовать в отношении только один раз — то есть ни в какой другой строке отношения не может быть значений, равных данным.
Так как [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-NULL)_[значения NULL](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-NULL "NULL")_ не считаются равными друг другу, ограничение уникальности не нарушается, если в отношении есть несколько строк со значениями NULL.

Ограничение-проверка
Вид [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-CONSTRAINT)_[ограничения](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-CONSTRAINT "Ограничение")_, определяемый для [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION)_[отношения](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION "Отношение")_ и ограничивающий множество значений, допустимых в одном или нескольких [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-ATTRIBUTE)_[атрибутах](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-ATTRIBUTE "Атрибут")_. Проверка-ограничение может обращаться к любому атрибуту в той же строке отношения, но не может обращаться к другим строкам этого же отношения или к другим отношениям.
Подробности в [Разделе 5.5](https://postgrespro.ru/docs/postgresql/current/ddl-constraints.html "5.5. Ограничения").

Оконная функция (подпрограмма)
Вид [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-FUNCTION)_[функций](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-FUNCTION "Функция (подпрограмма)")_, используемых в [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-QUERY)_[запросах](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-QUERY "Запрос")_, который применяется к [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-PARTITION)_[секции](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-PARTITION "Секция")_ [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RESULT-SET)_[результирующего множества](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RESULT-SET "Результирующее множество")_ запроса; результат такой функции зависит от значений в [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TUPLE)_[строках](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TUPLE "Кортеж")_ одной секции или рамки.
В качестве оконных могут использоваться и [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-AGGREGATE)_[агрегатные функции](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-AGGREGATE "Агрегатная функция (подпрограмма)")_, но оконные функции способны, например, определять ранг для каждой строки в секции. Также они называются _аналитическими функциями_.
Подробности в [Разделе 3.5](https://postgrespro.ru/docs/postgresql/current/tutorial-window.html "3.5. Оконные функции").

Оптимизатор
См. [Планировщик запросов](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-PLANNER).

Отношение
Общий термин, который охватывает все объекты в [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE)_[базе данных](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE "База данных")_, имеющие имя и упорядоченный список [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-ATTRIBUTE)_[атрибутов](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-ATTRIBUTE "Атрибут")_. Отношениями являются [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE)_[таблицы](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE "Таблица")_, [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SEQUENCE)_[последовательности](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SEQUENCE "Последовательность (отношение)")_, [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-VIEW)_[представления](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-VIEW "Представление")_, [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-FOREIGN-TABLE)_[сторонние таблицы](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-FOREIGN-TABLE "Сторонняя таблица (отношение)")_, [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-MATERIALIZED-VIEW)_[материализованные представления](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-MATERIALIZED-VIEW "Материализованное представление (отношение)")_, составные типы и [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-INDEX)_[индексы](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-INDEX "Индекс (отношение)")_.
В более общем смысле отношением является набор кортежей; например, результат выполнения запроса тоже отношение.
В PostgreSQL название _класс_ является устаревшим синонимом _отношения_.

Очистка (VACUUM)
Процесс удаления устаревших [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TUPLE)_[версий кортежей](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TUPLE "Кортеж")_ из таблиц или материализованных представлений и другая тесно связанная с ним обработка данных, потребность в которой продиктована реализацией [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-MVCC)_[MVCC](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-MVCC "Многоверсионное управление конкурентным доступом (MVCC)")_ в PostgreSQL. Очистку можно запустить вручную, воспользовавшись командой `VACUUM`, но она также может осуществляться автоматически процессами [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-AUTOVACUUM)_[автоочистки](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-AUTOVACUUM "Автоочистка (autovacuum)")_.
Подробности в [Разделе 24.1](https://postgrespro.ru/docs/postgresql/current/routine-vacuuming.html "24.1. Регламентная очистка").

Параллельное выполнение
Возможность распределять обработку частей [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-QUERY)_[запроса](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-QUERY "Запрос")_ между несколькими процессами, увеличивая тем самым эффективность использования многоядерных компьютеров.

Первичный ключ
Особый вид [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-UNIQUE-CONSTRAINT)_[ограничения уникальности](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-UNIQUE-CONSTRAINT "Ограничение уникальности")_, определяемого для [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE)_[таблицы](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE "Таблица")_ или другого [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION)_[отношения](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION "Отношение")_, который дополнительно гарантирует, что все [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-ATTRIBUTE)_[атрибуты](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-ATTRIBUTE "Атрибут")_ в [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-PRIMARY-KEY)_[первичном ключе](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-PRIMARY-KEY "Первичный ключ")_ отличны от [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-NULL)_[null](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-NULL "NULL")_. Как можно понять из названия, в таблице может быть только один первичный ключ, хотя в ней может быть несколько ограничений уникальности, так же не допускающих значения null в атрибутах.

Переработка
См. [Файл WAL](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL-FILE).

Планировщик запросов
Компонент PostgreSQL, предназначенный для определения (_планирования_) наиболее эффективного способа выполнения [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-QUERY)_[запросов](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-QUERY "Запрос")_. Также называется _оптимизатором запросов_, _оптимизатором_ или просто _планировщиком_.

Подпрограмма
Определённый набор инструкций, сохранённый в СУБД, который может выполняться по запросу. Подпрограммы могут быть написаны на самых разных языках программирования. Понятие подпрограмм включает [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-FUNCTION)_[функции](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-FUNCTION "Функция (подпрограмма)")_ (в том числе функции, возвращающие множества, и [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TRIGGER)_[триггерные функции](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TRIGGER "Триггер")_), [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-AGGREGATE)_[агрегатные функции](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-AGGREGATE "Агрегатная функция (подпрограмма)")_ и [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-PROCEDURE)_[процедуры](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-PROCEDURE "Процедура (подпрограмма)")_.
PostgreSQL уже содержит большое количество подпрограмм и при этом поддерживает добавление пользовательских подпрограмм.

Пользователь
[](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-ROLE)_[Роль](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-ROLE "Роль")_ с _правом LOGIN_ (см. [Раздел 21.2](https://postgrespro.ru/docs/postgresql/current/role-attributes.html "21.2. Атрибуты ролей")).

Последовательность (отношение)
Вид отношения, позволяющий генерировать значения, чаще всего это последовательные неповторяющиеся числа. Последовательности часто применяются для генерирования идентификаторов в [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-PRIMARY-KEY)_[первичном ключе](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-PRIMARY-KEY "Первичный ключ")_.

Последовательный номер в журнале (LSN)
Байтовое смещение в [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL)_[WAL](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL "Журнал предзаписи")_, монотонно увеличивающееся с каждой новой [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL-RECORD)_[записью WAL](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL-RECORD "Запись WAL")_.
Подробности в описании [`pg_lsn`](https://postgrespro.ru/docs/postgresql/current/datatype-pg-lsn.html "8.20. Тип pg_lsn") и [Раздел 28.6](https://postgrespro.ru/docs/postgresql/current/wal-internals.html "28.6. Внутреннее устройство WAL").

Представление
[](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION)_[Отношение](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION "Отношение")_, которое определяется оператором `SELECT` но само по себе не хранится. При каждом обращении к представлению его определение подставляется в запрос, как если бы пользователь просто вставил это определение в запрос вместо имени представления.
Подробности в описании [CREATE VIEW](https://postgrespro.ru/docs/postgresql/current/sql-createview.html "CREATE VIEW").

Приведение
Преобразование [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATUM)_[элемента данных](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATUM "Элемент данных")_ из его текущего типа в другой тип данных.
Подробности в [CREATE CAST](https://postgrespro.ru/docs/postgresql/current/sql-createcast.html "CREATE CAST").

Процедура (подпрограмма)
Вид подпрограммы, характеризующийся отсутствием возвращаемых значений. Кроме того, процедуры могут содержать операторы управления транзакциями, например `COMMIT` и `ROLLBACK`. Вызываются процедуры командой `CALL`.
Подробности в описании [CREATE PROCEDURE](https://postgrespro.ru/docs/postgresql/current/sql-createprocedure.html "CREATE PROCEDURE").

Процесс postmaster
Самый первый процесс [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-INSTANCE)_[экземпляра](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-INSTANCE "Экземпляр СУБД")_ сервера. Он запускает [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-AUXILIARY-PROC)_[вспомогательные процессы](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-AUXILIARY-PROC "Вспомогательный процесс")_ и управляет ими, а также создаёт [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-BACKEND)_[обслуживающие процессы](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-BACKEND "Обслуживающий процесс (backend)")_ по требованию.
Подробности в [Разделе 18.3](https://postgrespro.ru/docs/postgresql/current/server-start.html "18.3. Запуск сервера баз данных").

Процесс архивации WAL
[](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-AUXILIARY-PROC)_[Вспомогательный процесс](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-AUXILIARY-PROC "Вспомогательный процесс")_, который сохраняет копии [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL-FILE)_[файлов WAL](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL-FILE "Файл WAL")_ для осуществления резервного копирования или для поддержания актуального состояния [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-REPLICA)_[реплик](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-REPLICA "Реплика")_. Он может быть отключён.
Подробности в [Разделе 25.3](https://postgrespro.ru/docs/postgresql/current/continuous-archiving.html "25.3. Непрерывное архивирование и восстановление на момент времени (Point-in-Time Recovery, PITR)").

Процесс записи WAL
[](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-AUXILIARY-PROC)_[Вспомогательный процесс](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-AUXILIARY-PROC "Вспомогательный процесс")_, который переносит [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL-RECORD)_[записи WAL](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL-RECORD "Запись WAL")_ из [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SHARED-MEMORY)_[общей памяти](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SHARED-MEMORY "Общая память")_ в [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL-FILE)_[файлы WAL](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL-FILE "Файл WAL")_.
Подробности в описании [Разделе 19.5](https://postgrespro.ru/docs/postgresql/current/runtime-config-wal.html "19.5. Журнал предзаписи").

Процесс запуска
[](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-AUXILIARY-PROC)_[Вспомогательный процесс](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-AUXILIARY-PROC "Вспомогательный процесс")_, воспроизводящий WAL во время восстановления после сбоя и в [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-REPLICATION)_[физической реплике](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-REPLICATION "Репликация")_.
(Такое имя объясняется историческими причинами: процесс запуска был назван так до того, как была реализована репликация; имя отражает задачу этого процесса — запуск сервера после сбоя.)

Процесс контрольных точек (checkpointer)
[](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-AUXILIARY-PROC)_[Вспомогательный процесс](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-AUXILIARY-PROC "Вспомогательный процесс")_, отвечающий за выполнение процедуры [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-CHECKPOINT)_[контрольной точки](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-CHECKPOINT "Контрольная точка")_.

Процесс протоколирования
[](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-AUXILIARY-PROC)_[Вспомогательный процесс](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-AUXILIARY-PROC "Вспомогательный процесс")_, который записывает сообщения о событиях в базе данных в свой текущий [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-LOG-FILE)_[файл журнала](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-LOG-FILE "Файл журнала")_. Данный файл сменяется другим, когда выполняется некоторый критерий (ограничение по времени или объёму). Также этот процесс называется _syslogger_. Он может быть отключён.
Подробности в [Разделе 19.8](https://postgrespro.ru/docs/postgresql/current/runtime-config-logging.html "19.8. Регистрация ошибок и протоколирование работы сервера").

Процесс создания сводок WAL
[](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-AUXILIARY-PROC)_[Вспомогательный процесс](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-AUXILIARY-PROC "Вспомогательный процесс")_, отвечающий за создание сводок данных WAL для [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-INCREMENTAL-BACKUP)_[инкрементальных резервных копий](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-INCREMENTAL-BACKUP "Инкрементальная резервная копия")_.
Подробности в описании [Подраздел 19.5.7](https://postgrespro.ru/docs/postgresql/current/runtime-config-wal#RUNTIME-CONFIG-WAL-SUMMARIZATION "19.5.7. Создание сводок WAL").

Процесс фоновой записи
[](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-AUXILIARY-PROC)_[Вспомогательный процесс](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-AUXILIARY-PROC "Вспомогательный процесс")_, записывающий «грязные» [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATA-PAGE)_[страницы данных](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATA-PAGE "Страница данных")_ из [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SHARED-MEMORY)_[общей памяти](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SHARED-MEMORY "Общая память")_ в файловую систему. Он периодически активируется на короткое время, чтобы создаваемая им значительная нагрузка на подсистему ввода-вывода распределялась во времени с целью исключения пиков нагрузки, блокирующих другие процессы.
Подробности в [Подразделе 19.4.4](https://postgrespro.ru/docs/postgresql/current/runtime-config-resource#RUNTIME-CONFIG-RESOURCE-BACKGROUND-WRITER "19.4.4. Фоновая запись").

Процесс-передатчик WAL
Специальный [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-BACKEND)_[обслуживающий процесс](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-BACKEND "Обслуживающий процесс (backend)")_, передающий WAL по сети. Принимать его может [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL-RECEIVER)_[процесс-приёмник WAL](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL-RECEIVER "Процесс-приёмник WAL")_ в [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-REPLICA)_[реплике](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-REPLICA "Реплика")_, [pg_receivewal](https://postgrespro.ru/docs/postgresql/current/app-pgreceivewal.html "pg_receivewal") или любая другая клиентская программа, понимающая протокол репликации.

Процесс-приёмник WAL
[](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-AUXILIARY-PROC)_[Вспомогательный процесс](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-AUXILIARY-PROC "Вспомогательный процесс")_, который выполняется на [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-REPLICA)_[реплике](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-REPLICA "Реплика")_ и получает от [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-PRIMARY-SERVER)_[основного сервера](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-PRIMARY-SERVER "Ведущий (сервер)")_ WAL для воспроизведения [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-STARTUP-PROCESS)_[процессом запуска](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-STARTUP-PROCESS "Процесс запуска")_.
Подробности в [Разделе 26.2](https://postgrespro.ru/docs/postgresql/current/warm-standby.html "26.2. Трансляция журналов на резервные серверы").

Раздувание
Увеличение объёма, занимаемого не текущими версиями строк, в том числе объёма неиспользуемого (свободного) места и объёма, занимаемого устаревшими версиями строк.

Расширение

Дополнительный программный модуль, который может быть установлен в [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-INSTANCE)_[экземпляре](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-INSTANCE "Экземпляр СУБД")_ сервера для расширения его функциональности.
Подробности в [Разделе 36.17](https://postgrespro.ru/docs/postgresql/current/extend-extensions.html "36.17. Упаковка связанных объектов в расширение").

Результирующее множество

[](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION)_[Отношение](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION "Отношение")_, передаваемое из [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-BACKEND)_[обслуживающего процесса](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-BACKEND "Обслуживающий процесс (backend)")_ [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-CLIENT)_[клиенту](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-CLIENT "Клиент (процесс)")_ после выполнения команды SQL, обычно `SELECT`, но также это могут быть команды `INSERT`, `UPDATE`, `DELETE` или `MERGE` с предложением `RETURNING`.
То, что результирующее множество является отношением, означает, что один запрос может фигурировать в определении другого запроса в качестве _подзапроса_.

Реплика

[](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE)_[База данных](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE "База данных")_, связанная с [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-PRIMARY-SERVER)_[ведущей](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-PRIMARY-SERVER "Ведущий (сервер)")_ базой и содержащая копию некоторых или всех данных последней. Прежде всего такие базы создаются для расширения возможностей доступа к данным, а также для обеспечения доступности данных в случае потери [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-PRIMARY-SERVER)_[ведущего сервера](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-PRIMARY-SERVER "Ведущий (сервер)")_.

Репликация
Перенос информации с одного [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SERVER)_[сервера](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SERVER "Сервер")_ на другой называется [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-REPLICA)_[репликацией](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-REPLICA "Реплика")_. Она может реализовываться как _физическая репликация_, когда с одного сервера на другой переносятся все изменения на уровне файлов, или как _логическая репликация_, когда передаются изменения в определённом подмножестве данных, представленные на более высоком уровне.

Роль
Набор прав доступа к объектам [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE)_[экземпляра](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE "База данных")_ сервера. Принадлежность к роли тоже может считаться правом, которым можно наделять другие роли. Это часто используется, когда нужно дать одинаковые права множеству [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-USER)_[пользователей](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-USER "Пользователь")_ или организовать распределение прав удобным образом.
Подробности в описании [CREATE ROLE](https://postgrespro.ru/docs/postgresql/current/sql-createrole.html "CREATE ROLE").

Сеанс
Состояние, в котором клиент может взаимодействовать с обслуживающим процессом, используя установленное [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-CONNECTION)_[соединение](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-CONNECTION "Соединение")_.

Сегмент
См. [Файловый сегмент](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-FILE-SEGMENT).

Сегмент WAL
См. [Файл WAL](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL-FILE).

Секционированная таблица (отношение)
[](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION)_[Отношение](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION "Отношение")_, которое по смыслу не отличается от [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE)_[таблицы](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE "Таблица")_, но его содержимое хранится распределённо, в нескольких [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-PARTITION)_[секциях](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-PARTITION "Секция")_.

Секция
Одно из нескольких отдельных (не пересекающихся) подмножеств большего множества.
Применительно к [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-PARTITIONED-TABLE)_[секционированной таблице](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-PARTITIONED-TABLE "Секционированная таблица (отношение)")_: одна из таблиц, содержащих часть данных секционированной таблицы, которая называется _родительской_. Секция сама по себе является таблицей, поэтому запросы могут обращаться к ней напрямую; при этом секция тоже может быть секционированной таблицей, таким образом могут создаваться иерархии.
Применительно к [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WINDOW-FUNCTION)_[оконным функциям](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WINDOW-FUNCTION "Оконная функция (подпрограмма)")_ в [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-QUERY)_[запросе](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-QUERY "Запрос")_ секция соответствует определённому пользователем критерию, группирующему [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TUPLE)_[строки](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TUPLE "Кортеж")_ [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RESULT-SET)_[результирующего множества запроса](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RESULT-SET "Результирующее множество")_ для обработки такой функцией.

Сервер
Компьютер, на котором работают [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-INSTANCE)_[экземпляры](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-INSTANCE "Экземпляр СУБД")_ PostgreSQL. _Сервером_ может называться как физическая, так и _виртуальная машина_ или контейнер.
Иногда сервером также называют экземпляр сервера баз данных.

Сервер баз данных
См. [Экземпляр СУБД](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-INSTANCE).

Сетевой узел (host)
Компьютер, взаимодействующий с другими компьютерами по сети. Иногда так называют [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SERVER)_[сервер](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SERVER "Сервер")_. Также это название применимо к компьютеру, на котором работают [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-CLIENT)_[клиентские процессы](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-CLIENT "Клиент (процесс)")_.

Система накопительной статистики
Система, которая собирает статистическую информацию о действиях [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-INSTANCE)_[экземпляра](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-INSTANCE "Экземпляр СУБД")_ сервера. Она может быть отключена.
Подробности в [Разделе 27.2](https://postgrespro.ru/docs/postgresql/current/monitoring-stats.html "27.2. Система накопительной статистики").

Системный каталог
Набор [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE)_[таблиц](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE "Таблица")_, которые описывают структуру всех [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SQL-OBJECT)_[SQL-объектов](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SQL-OBJECT "SQL-объект")_ сервера. Системный каталог располагается в схеме `pg_catalog`. Его таблицы содержат данные во внутреннем представлении и не считаются полезными для конечных пользователей. В более понятном виде часть этой информации доступна в ряде системных [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-VIEW)_[представлений](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-VIEW "Представление")_, также находящихся в схеме `pg_catalog`. Кроме того, имеется схема `information_schema` (см. [Главу 35](https://postgrespro.ru/docs/postgresql/current/information-schema.html "Глава 35. Информационная схема")), содержащая дополнительные таблицы и представления, из которых можно получить информацию (частично ту же, но также и некоторую другую), предоставляемую в соответствии с требованиями [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SQL-STANDARD)_[стандарта SQL](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SQL-STANDARD "Стандарт SQL")_.
Подробности в [Разделе 5.10](https://postgrespro.ru/docs/postgresql/current/ddl-schemas.html "5.10. Схемы").

Слой
Отдельный набор файлов-сегментов, в которых хранится отношение. В _основном слое_ находятся собственно данные отношения. Помимо него существует два дополнительных слоя для метаданных: [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-FSM)_[карта свободного пространства](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-FSM "Карта свободного пространства (слой)")_ и [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-VM)_[карта видимости](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-VM "Карта видимости (слой)")_. У [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-UNLOGGED)_[нежурналируемых отношений](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-UNLOGGED "Нежурналируемое отношение")_ также имеется _слой инициализации_.

Согласованность
Свойство [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE)_[базы](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE "База данных")_, суть которого в том, что данные базы всегда удовлетворяют [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-CONSTRAINT)_[ограничениям целостности](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-CONSTRAINT "Ограничение")_. Транзакциям позволяется временно нарушать такие ограничения, но если к моменту завершения транзакции эти нарушения не устраняются, транзакция автоматически [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-ROLLBACK)_[откатывается](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-ROLLBACK "ROLLBACK")_. Это одно из свойств ACID.

Соединение
Установленное подключение клиентского процесса к [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-BACKEND)_[обслуживающему](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-BACKEND "Обслуживающий процесс (backend)")_ процессу, обычно сетевое, в рамках которого существует [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SESSION)_[сеанс](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SESSION "Сеанс")_. Иногда этот термин употребляется как синоним сеанса.
Подробности в [Разделе 19.3](https://postgrespro.ru/docs/postgresql/current/runtime-config-connection.html "19.3. Подключения и аутентификация").

Соединение (join)
Операция (и ключевое слово SQL), выполняемая в [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-QUERY)_[запросах](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-QUERY "Запрос")_ для объединения данных из нескольких [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION)_[отношений](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION "Отношение")_.

Сопоставление пользователей
Устанавливаемое в [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-FOREIGN-DATA-WRAPPER)_[обёртке сторонних данных](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-FOREIGN-DATA-WRAPPER "Обёртка сторонних данных")_ соответствие учётной записи в локальной [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE)_[базе данных](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE "База данных")_ другой учётной записи в удалённой системе.
Подробности в описании [CREATE USER MAPPING](https://postgrespro.ru/docs/postgresql/current/sql-createusermapping.html "CREATE USER MAPPING").

Ссылочная целостность
Средство ограничения данных в [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION)_[отношении](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION "Отношение")_ по [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-FOREIGN-KEY)_[внешнему ключу](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-FOREIGN-KEY "Внешний ключ")_ таким образом, чтобы им обязательно соответствовали данные в другом [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION)_[отношении](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION "Отношение")_.

Стандарт SQL
Совокупность документов, определяющих язык SQL.

Столбец
[](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-ATTRIBUTE)_[Атрибут](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-ATTRIBUTE "Атрибут")_, относящийся к [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE)_[таблице](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE "Таблица")_ или [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-VIEW)_[представлению](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-VIEW "Представление")_.

Сторонний сервер
Именованный набор [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-FOREIGN-TABLE)_[сторонних таблиц](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-FOREIGN-TABLE "Сторонняя таблица (отношение)")_, для обращения к которым используется одна [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-FOREIGN-DATA-WRAPPER)_[обёртка сторонних данных](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-FOREIGN-DATA-WRAPPER "Обёртка сторонних данных")_ и общие параметры конфигурации.
Подробности в описании [CREATE SERVER](https://postgrespro.ru/docs/postgresql/current/sql-createserver.html "CREATE SERVER").

Сторонняя таблица (отношение)
[](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION)_[Отношение](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION "Отношение")_, [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TUPLE)_[строки](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TUPLE "Кортеж")_ и [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-COLUMN)_[столбцы](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-COLUMN "Столбец")_ которого представляются содержащимися в обычной [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE)_[таблице](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE "Таблица")_, но запросы к нему проходят через [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-FOREIGN-DATA-WRAPPER)_[обёртку сторонних данных](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-FOREIGN-DATA-WRAPPER "Обёртка сторонних данных")_. В ответ эта обёртка возвращает [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RESULT-SET)_[результирующие множества](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RESULT-SET "Результирующее множество")_, структурированные согласно определению [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-FOREIGN-TABLE)_[сторонних таблиц](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-FOREIGN-TABLE "Сторонняя таблица (отношение)")_.
Подробности в описании [CREATE FOREIGN TABLE](https://postgrespro.ru/docs/postgresql/current/sql-createforeigntable.html "CREATE FOREIGN TABLE").

Страница данных
Основная структура, в которой хранятся данные отношений. Все страницы имеют одинаковый размер. Страницы данных обычно хранятся на диске в определённых файлах и могут быть прочитаны в [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SHARED-MEMORY)_[общие буферы](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SHARED-MEMORY "Общая память")_, а затем претерпеть изменения, в результате которых они станут _грязными_. При записи на диск они вновь становятся чистыми. Новые страницы, изначально существующие только в памяти, также считаются грязными, пока не будут записаны на диск.

Стратегия доступа к буферу

Некоторые операции обращаются к большому количеству [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATA-PAGE)_[страниц](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATA-PAGE "Страница данных")_. _Стратегия доступа к буферу_ помогает предотвратить вытеснение из [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SHARED-MEMORY)_[общих буферов](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SHARED-MEMORY "Общая память")_ слишком большого количества страниц в результате этих операций.
Стратегия доступа к буферу устанавливает ссылки на ограниченное количество [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SHARED-MEMORY)_[общих буферов](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SHARED-MEMORY "Общая память")_ и использует их циклически. Когда для операции требуется новая страница, целевой буфер выбирается из буферов в стратегическом цикле, что может потребовать сброса «грязных» данных страницы и, возможно, также несброшенного [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL)_[WAL](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL "Журнал предзаписи")_ в постоянное хранилище.
Стратегии доступа к буферу используются для различных операций, таких как последовательное сканирование больших таблиц, `VACUUM`, `COPY`, `CREATE TABLE AS SELECT`, `ALTER TABLE`, `CREATE DATABASE`, `CREATE INDEX` и `CLUSTER`.

Строка таблицы
См. [Кортеж](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TUPLE).

Суперпользователь
В данной документации это синоним [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE-SUPERUSER)_[суперпользователя базы данных](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE-SUPERUSER "Суперпользователь баз данных")_.

Суперпользователь баз данных
Роль, имеющая _статус суперпользователя_ (см. [Раздел 21.2](https://postgrespro.ru/docs/postgresql/current/role-attributes.html "21.2. Атрибуты ролей")).
Часто также называется _суперпользователь_.

Схема
Пространство имён [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SQL-OBJECT)_[SQL-объектов](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SQL-OBJECT "SQL-объект")_, принадлежащих одной [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE)_[базе данных](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE "База данных")_. Каждый отдельный SQL-объект должен располагаться ровно в одной схеме.
Все системные SQL-объекты располагаются в схеме `pg_catalog`.
В более общем смысле _схема_ — это совокупность всех описаний данных (определений [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE)_[таблиц](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TABLE "Таблица")_, [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-CONSTRAINT)_[ограничений](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-CONSTRAINT "Ограничение")_, комментариев и т. д.) в определённой [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE)_[базе](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE "База данных")_ или в её подмножестве.
Подробности в [Разделе 5.10](https://postgrespro.ru/docs/postgresql/current/ddl-schemas.html "5.10. Схемы").

Таблица
Набор [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TUPLE)_[кортежей](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TUPLE "Кортеж")_, имеющих общую структуру данных (одинаковое количество [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-ATTRIBUTE)_[атрибутов](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-ATTRIBUTE "Атрибут")_ в том же порядке, имеющих одинаковые имена и типы). Таблица является наиболее распространённым видом [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION)_[отношения](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION "Отношение")_ в PostgreSQL.
Подробности в описании [CREATE TABLE](https://postgrespro.ru/docs/postgresql/current/sql-createtable.html "CREATE TABLE").

Табличное пространство
Именованное расположение в файловой системе сервера. Все [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SQL-OBJECT)_[SQL-объекты](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SQL-OBJECT "SQL-объект")_, для которых требуется хранилище, должны располагаться в некотором табличном пространстве (при этом их определения размещаются в [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SYSTEM-CATALOG)_[системном каталоге](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SYSTEM-CATALOG "Системный каталог")_). Изначально в кластере баз данных есть только одно табличное пространство, которое называется `pg_default` и содержит по умолчанию все SQL-объекты.
Подробности в [Разделе 22.6](https://postgrespro.ru/docs/postgresql/current/manage-ag-tablespaces.html "22.6. Табличные пространства").

Точка перезапуска
Вариант [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-CHECKPOINT)_[контрольной точки](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-CHECKPOINT "Контрольная точка")_, выполняемый на [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-REPLICA)_[реплике](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-REPLICA "Реплика")_.
Подробности в [Разделе 28.5](https://postgrespro.ru/docs/postgresql/current/wal-configuration.html "28.5. Настройка WAL").

Точка сохранения
Специальная отметка в последовательности операций [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TRANSACTION)_[транзакции](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TRANSACTION "Транзакция")_. Изменения данных, произведённые после этой отметки, могут быть отменены, таким образом будет получено состояние на момент сохранения.
Подробности в описании [SAVEPOINT](https://postgrespro.ru/docs/postgresql/current/sql-savepoint.html "SAVEPOINT").

Транзакции/сек (TPS)
Среднее количество транзакций, выполняющихся за секунду, подсчитанное по всем сеансам за время наблюдения. Эта величина позволяет оценить производительность экземпляра сервера.

Транзакция
Совокупность команд, которые должны выполниться как одна [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-ATOMIC)_[атомарная](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-ATOMIC "Атомарный")_ команда: они завершаются успешно либо отменяются все вместе, а результат их выполнения не виден в других [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SESSION)_[сеансах](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SESSION "Сеанс")_ до завершения транзакции и, возможно, даже позже (в зависимости от уровня изоляции)
Подробности в [Разделе 13.2](https://postgrespro.ru/docs/postgresql/current/transaction-iso.html "13.2. Изоляция транзакций").

Триггер
[](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-FUNCTION)_[Функция](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-FUNCTION "Функция (подпрограмма)")_, которая вызывается при выполнении определённой операции (`INSERT`, `UPDATE`, `DELETE`, `TRUNCATE`) с некоторым [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION)_[отношением](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION "Отношение")_. Триггер выполняется в рамках той же [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TRANSACTION)_[транзакции](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TRANSACTION "Транзакция")_, что и вызвавший его оператор, и если в функции триггера произойдёт ошибка, этот оператор тоже не будет выполнен успешно.
Подробности в описании [CREATE TRIGGER](https://postgrespro.ru/docs/postgresql/current/sql-createtrigger.html "CREATE TRIGGER").

Файл WAL
Также называется _сегментом WAL_ или _файлом сегмента WAL_. Представляет собой один из последовательно нумеруемых файлов, служащих хранилищем [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL)_[WAL](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL "Журнал предзаписи")_. Все эти файлы имеют одинаковый предопределённый размер и записываются по порядку. В файле WAL перемежаются изменения, производимые в нескольких параллельных сеансах. В случае сбоя системы эти файлы также по порядку считываются и все записанные в них изменения воспроизводятся, в результате чего восстанавливается последнее состояние системы до сбоя.
Каждый файл WAL может быть освобождён после того, как во время [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-CHECKPOINT)_[контрольной точки](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-CHECKPOINT "Контрольная точка")_ все изменения из него будут переписаны в соответствующие файлы данных. Освобождённый файл может быть просто удалён либо переименован (или _переработан_) так, чтобы его можно было использовать в будущем.
Подробности в [Разделе 28.6](https://postgrespro.ru/docs/postgresql/current/wal-internals.html "28.6. Внутреннее устройство WAL").

Файл журнала
Файлы журналов содержат предназначенные для человека текстовые сообщения о событиях. Например, в журнале могут фиксироваться ошибки входа, длительные запросы и т. д.
Подробности в [Разделе 24.3](https://postgrespro.ru/docs/postgresql/current/logfile-maintenance.html "24.3. Обслуживание журнала").

Файловый сегмент
Физический файл, содержащий данные для определённого [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION)_[отношения](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RELATION "Отношение")_. Размер сегментов ограничивается параметром конфигурации (обычно ограничение равно 1 гигабайту), поэтому отношения большего объёма разбиваются на несколько сегментов.
Подробности в [Разделе 66.1](https://postgrespro.ru/docs/postgresql/current/storage-file-layout.html "66.1. Размещение файлов базы данных").

(Не путайте это понятие с подобным понятием [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL-FILE)_[сегмент WAL](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-WAL-FILE "Файл WAL")_).

Фиксирование
Акт успешного завершения [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TRANSACTION)_[транзакции](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TRANSACTION "Транзакция")_ в [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE)_[базе данных](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DATABASE "База данных")_, обеспечивающий [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DURABILITY)_[надёжность](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DURABILITY "Надёжность")_ и видимость её результатов для других транзакций.
Подробности в [COMMIT](https://postgrespro.ru/docs/postgresql/current/sql-commit.html "COMMIT").

Фоновый рабочий процесс
Процесс внутри [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-INSTANCE)_[экземпляра](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-INSTANCE "Экземпляр СУБД")_ сервера, выполняющий системный или пользовательский код. Обеспечивает инфраструктуру для различной функциональности PostgreSQL, в частности для [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-REPLICATION)_[логической репликации](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-REPLICATION "Репликация")_ и [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-PARALLEL-QUERY)_[параллельных запросов](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-PARALLEL-QUERY "Параллельное выполнение")_. Кроме того, отдельные рабочие процессы могут создаваться [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-EXTENSION)_[расширениями](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-EXTENSION "Расширение")_.
Подробности в [Главе 46](https://postgrespro.ru/docs/postgresql/current/bgworker.html "Глава 46. Фоновые рабочие процессы").

Функция (подпрограмма)
Вид подпрограммы, который получает ноль или более аргументов, выдаёт ноль или более выходных значений и может выполняться только в рамках одной транзакции. Функции могут вызываться в ходе выполнения запросов, например, `SELECT`. Функции особого рода могут выдавать [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RESULT-SET)_[множества](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-RESULT-SET "Результирующее множество")_; они называются _функциями, возвращающими множества_.
Функции также вызываются при срабатывании [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TRIGGER)_[триггеров](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-TRIGGER "Триггер")_.
Подробности в описании [CREATE FUNCTION](https://postgrespro.ru/docs/postgresql/current/sql-createfunction.html "CREATE FUNCTION").

Экземпляр СУБД
Группа [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-BACKEND)_[обслуживающих](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-BACKEND "Обслуживающий процесс (backend)")_ и [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-AUXILIARY-PROC)_[вспомогательных процессов](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-AUXILIARY-PROC "Вспомогательный процесс")_, использующих общую область разделяемой памяти. Экземпляром СУБД управляет один [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-POSTMASTER)_[процесс postmaster](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-POSTMASTER "Процесс postmaster")_, и относится к этому экземпляру ровно один [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DB-CLUSTER)_[кластер баз данных](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-DB-CLUSTER "Кластер баз данных")_ со всеми его базами. На одном [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SERVER)_[сервере](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-SERVER "Сервер")_ могут работать несколько экземпляров СУБД, если их TCP-порты не конфликтуют.
Конкретный экземпляр реализует все функциональные возможности СУБД: читает и записывает файлы, работает с общей памятью, обеспечивает свойства ACID, принимает [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-CONNECTION)_[подключения](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-CONNECTION "Соединение")_ [](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-CLIENT)_[клиентских процессов](https://postgrespro.ru/docs/postgresql/current/glossary#GLOSSARY-CLIENT "Клиент (процесс)")_, проверяет права доступа, выполняет восстановление после сбоя, осуществляет репликацию и т. д.

Элемент данных
Внутреннее представление одного значения некоторого типа данных SQL.

