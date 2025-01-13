# QA_Load
# Test_task: QA Performance 13.01.2025

## Описание
Данное тестовое задание включает разработку Java-приложения и выполнение нагрузочного тестирования с использованием Apache JMeter.

## Использованные технологии
- Java (Spring Boot)
- Apache Kafka
- PostgreSQL
- Apache JMeter

## Структура проекта

- `jmeter/Kafka_Axen.jmx` — файл с тестовым сценарием JMeter
- `docs/Test_task_13.01.2025.docx` — полное описание задания
- `docs/Release_test_task_13.01.2025.docx` — отчет о реализации задания
- `logs/DBt.txt` — результаты SQL-запросов и анализа БД
  
## Запуск и использование
1. **Настройка Kafka и PostgreSQL:**
   - Запуск Kafka и создание топика `Franz_Kafka`
   - Настройка БД PostgreSQL, убедиться, что доступна база `antares_db`

2. **Запуск Java-приложения:**
   ```sh
   java -jar target/kafkalistener-0.0.1-SNAPSHOT.jar
   ```
запуск jar.файла по 
ссылке на приложение 
https://github.com/verakolkutina/kafkalistener_01.git

4. **Запуск JMeter-тестов:**
   - Откройте `Kafka_Axen.jmx` в Apache JMeter
   - Настройка параметров подключения
   - Запуск теста 

## Результаты тестирования
Основные команды для работы,выводы и анализ результатов тестирования отражены в файле `Release_test_task_13.01.2025.docx`.

## Вывод

Для задания были развернуты и настроены Kafka, Zookeeper и PostgreSQL, 
разработан тестовый сценарий на JMeter,а также разработана заглушка на Java (Spring), 
проведено тестирование Kafka с помощью JMeter, и выполнен анализ производительности SQL-запросов 
с помощью расширения pg_stat_statements: общее время было равно 115.74 мсек, а среднее время составляло 0.078 мсек.
