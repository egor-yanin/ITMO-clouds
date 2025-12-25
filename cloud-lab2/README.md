# Отчет по облачной лабораторной работе №2  

## Создание кросс-провайдерной модели AWS и Azure

### Вариант 7

## Цель работы

Получение навыков аналитики и понимания спектра публичных облачных сервисов без привязки к вендору. Формирование комплексного видения Облака.

В качестве базовой модели использовалась сервисная структура AWS, разработанная в лабораторной работе №1. Ее мы применили для классификации сервисов Microsoft Azure. Такжеиспользовалась официальная документация Microsoft Azure: https://learn.microsoft.com/azure/

## Выполнение работы

Чтобы выполнить поставленную задачу, нам необходимо было проанализировать сервисы Azure на основе `Meter Category`, `Meter Sub-Category` и `Meter Name`, из биллинговых данных и наийти аналог в модели AWS и сопоставить значения с уже существующими праметрами классификации.

Для каждой строки данных были заполнены следующие классификационные атрибуты:
- IT Tower  
- Service Family  
- Service Type  
- Service Sub Type  
- Service Usage Type  

## Теория

В рамках лр используется униврсальная модель классификации облачных сервисов, в ее основе лежат три базовых подхода предоставления облачных услуг:

<img width="1418" height="740" alt="image" src="https://github.com/user-attachments/assets/aee586e2-1cea-4b2a-80b0-27d049176118" />

### IaaS (Infrastructure as a Service)

Модель, при которой облачный провайдер предоставляет базовые инфраструктурные ресурсы, а управление операционной системой и программным обеспечением выполняется пользователем

**Примеры сервисов в Azure:**
- Virtual Machines  
- Virtual Network  
- Load Balancer  

### PaaS (Platform as a Service)

Модель предоставления готовой платформы для разработки и развертывания приложений без управления инфраструктурой

**Примеры сервисов в Azure:**
- Azure App Service  
- Azure Container Instances  
- Azure Event Grid  
- Azure Service Bus  
- Azure IoT Hub  
- Azure Cognitive Services  
- Azure Machine Learning  

### SaaS (Software as a Service)

Модель предоставления готовых приложений, доступных через интернет, без необходимости управления инфраструктурой и платформой

**Примеры сервисов в Azure:**
- Dynamics 365 Customer Insights  
- Visual Studio / Azure DevOps  
## Классификация сервисов Microsoft Azure

### 1. Cloud Services  
*(Управляемые платформенные сервисы)*

#### Аналитика (Analytics)

**Azure SQL Database / Azure Synapse Analytics** — управляемые реляционные базы данных и аналитические хранилища.

- Использование: vCore, DTUs, Database Units, Storage  

Российский аналог: Yandex Managed Service for PostgreSQL, Postgres Pro (VK Cloud)

**Azure Data Factory v2** — сервис интеграции и оркестрации данных (ETL).

- Использование: Activity Runs, Data Movement, Pipeline Execution  

Российский аналог: Yandex Data Proc + Airflow / Yandex DataLens


#### Сервисы приложений (Application Services)

**Azure App Service (Websites)** — платформа для размещения и масштабирования веб-приложений.

- Использование: Hours, Free Tier, IP SSL  

Российский аналог: VK Cloud App Engine, Yandex Cloud Functions + API Gateway

**Visual Studio Team Services / Azure Application Insights** — инструменты DevOps и мониторинга приложений.

- Использование: Users, Agents, Insights  

Российский аналог: Yandex Tracker, Yandex Monitoring

### 2. Infrastructure  
*(Инфраструктура как услуга, IaaS)*

#### Вычисления (Compute)

**Azure Virtual Machines** — виртуальные серверы с различными конфигурациями и лицензиями ОС.

- Использование: Compute Hours  

Российский аналог: Yandex Compute Cloud, VK Cloud Virtual Machines

### 3. Storage  
*(Хранилища данных)*

**Azure Blob Storage / Azure Managed Disks** — объектное и блочное хранилище данных.

- Использование: Storage GB, Data Stored  

Российский аналог: Yandex Object Storage, Yandex Compute Cloud Disks

**Azure Backup / Azure Recovery Services Vault** — сервисы резервного копирования.

- Использование: Storage  

Российский аналог: Yandex Cloud Backup

# Выводы

В ходе лабораторной работы мы смогли применить модель на основе AWS для структурирования сервисов Microsoft Azure и создать единую кросс-провайдерную модель классификации облачных сервисов (а еще сложить глаза в кучу от количества информации в документации)
