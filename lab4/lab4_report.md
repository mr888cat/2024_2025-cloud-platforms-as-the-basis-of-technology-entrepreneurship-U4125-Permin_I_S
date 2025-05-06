# Лабораторная работа №3 «Разработка инфраструктуры MVP AI приложения»  
University: [ITMO University](https://itmo.ru/ru/)  
Faculty: [FTMI](https://itmo.ru/ru/viewfaculty/87/fakultet_tehnologicheskogo_menedzhmenta_i_innovaciy.htm)  
Course: [Cloud platforms as the basis of technology entrepreneurship](https://itmo-ict-faculty.github.io/cloud-platforms-as-the-basis-of-technology-entrepreneurship/)  
Year: 2024/2025  
Group: U4125  
Author: Permin Ivan Sergeevich
Lab: Lab4  
Date of create: 05.05.2025  
Date of finished:  06.05.2025
  
Для выполнения задания я выбрал сервис для продвижения в Телеграм. Сервис используется для продвижения каналов, товаров, чатов в Телеграм. С помощью искусственного интеллекта сервис будет проводить анализ конкурентов, автоматически оставлять комментарии под постами, а так же участвовать в дискуссиях в чатах.

|Элемент|Начальная фаза (MVP)|Тестирование с партнёрами|Продакшн (Production)|
|---|---|---|---|
|**Цель**|Прототип, тест идеи, минимальные затраты|Проверка нагрузки, партнёрский доступ|Масштабируемость, отказоустойчивость, монетизация|
|**Фронтенд**|Telegram Web App (React, Firebase Hosting)|Без изменений|Telegram Web App + аналитика использования|
|**Бэкенд**|1 Cloud Run сервис (256MB–512MB RAM)|Cloud Run (1GB RAM, 2vCPU) + Cloud Functions|Cloud Run с автошкалированием, приватный доступ|
|**База данных**|Firestore (NoSQL)|Firestore (увеличен лимит)|Firestore или Cloud SQL (если нужны транзакции)|
|**ИИ-интеграции**|ChatGPT, DeepSeek, Grok (через API)|Те же, + управление через очереди|Распределение AI-запросов, A/B тестирование|
|**Очереди / фоновые задачи**|Нет|Pub/Sub для анализа и AI-обработки|Cloud Tasks + Pub/Sub, асинхронная архитектура|
|**Платёжные шлюзы**|YooMoney|YooMoney + Stripe|Stripe + YooMoney (полный цикл оплаты и подписок)|
|**Мониторинг / Логи**|Cloud Logging (базовый)|Cloud Logging + базовый Monitoring|Logging, Monitoring, Error Reporting, Traces|
|**Аналитика**|Нет|Встроенные логи, basic дашборды|BigQuery + Looker или DataStudio|
|**Кэш / ускорение**|Нет|—|Redis (MemoryStore) для кэша AI-ответов и сессий|
|**Безопасность**|Открытый API|Секреты через Secret Manager|IAM, Secret Manager, ограничение входа в API|
|**Оценка нагрузки**|200 пользователей / 50 запросов в день|1000 пользователей / 300 запросов в день|10,000+ пользователей / 1000+ AI-запросов в день|
|**Стоимость** (примерно)|$20–40/мес|$50–120/мес|$300+/мес (в зависимости от AI и API использования)|



![image](https://github.com/user-attachments/assets/62942e5e-791d-420d-9491-2c562fb35d83)



![Pasted image 20250506181421](https://github.com/user-attachments/assets/0a178eef-b565-40a7-8cd1-6d8581bcedbf)


