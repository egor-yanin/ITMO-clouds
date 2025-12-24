# Отчёт по облачной лабораторной работе №1

Вариант 7

## Теория

<img width="870" height="473" alt="image" src="https://github.com/user-attachments/assets/2e562b05-b75c-4f00-8838-6bc68ec6f34f" />

**IaaS** (Infrastructure as a Service) — это предоставление вычислительных ресурсов в аренду сторонним компаниям.
Провайдер владеет и управляет IT-инфраструктурой, а его клиенты используют ее мощности для решения своих задач.

**SaaS** (Software as a Service) — это облачная модель предоставления программного обеспечения, в которой приложения и данные размещаются на удалённых серверах, а пользователи получают к ним доступ с помощью устройств, подключённых к интернету. Например, так работают мессенджеры. 
Пользователь устанавливает себе приложение, но при этом вся нужная информация — сообщения, фото, видео и контакты — хранится на серверах.

**PaaS** (Platform as a Service) — это способ предоставления вычислительных ресурсов в облаке, когда пользователь получает уже готовый сервис или платформу для запуска своего кода и хранения данных.
Облачный провайдер обеспечивает бесперебойную работу и автоматизированное управление инфраструктурой. 

## Сервисы

### Amazon Macie — SaaS
Сервис, который обнаруживает конфиденциальные данные и обеспечивает безопасность данных c помощью машинного обучения. Аналог - [Yandex Security Deck](https://yandex.cloud/ru/services/security-deck) в Yandex Cloud.

### Amazon MSK (Amazon Managed Streaming for Apache Kafka) — PaaS
Сервис, который используется для работы с приложениями, которые используют Apache Kafka - платформу для потоковой передачи и обработки данных. Аналог - [Yandex Managed Service for Apache Kafka](https://yandex.cloud/ru/services/managed-kafka) в Yandex Cloud, [Advanced Distributed Message Service for Kafka](https://cloud.ru/products/distributed-message-service-for-kafka) в cloud.ru.

### Amazon Polly — SaaS
Сервис для генерации голоса на базе искусственного интеллекта (TTS - Text-to-speech). Аналог - [Yandex SpeechKit](https://yandex.cloud/ru/services/speechkit).

### Amazon Personalize — SaaS
Ещё один сервис, который использует машинное обучение, на этот раз для генерации рекомендаций на основе данных пользователей. Аналог - [Yandex DataSphere](https://yandex.cloud/ru/blog/posts/2022/05/recommendation-system-instruction).

### Amazon S3 (Simple Storage Service) — IaaS
Сервис для храниения данных различного объёма. В файле биллинга используется Glacier, Glacier Deep Archive и Intelligent-Tiering, который разделяет данные на Frequent и Infrequent Access.
<img width="1154" height="653" alt="image" src="https://github.com/user-attachments/assets/6b86aeaf-3ea5-4a50-9b8f-a1b1c86329a0" />
Также начисляется штраф за удаление раньше срока - Early Delete.
Запросы различаются по стоимости в зависимости от их Tier.
Аналоги - [Yandex Object Storage](https://yandex.cloud/ru/services/storage), [Evolution Object Storage](https://cloud.ru/products/evolution-object-storage).

### Amazon OpenSearch Service (в таблице Amazon ES)
Сервис для поиска и аналитики информации, который использует опенсорсный OpenSearch. Аналог - [Yandex Managed Service for OpenSearch](https://yandex.cloud/ru/services/managed-opensearch).
