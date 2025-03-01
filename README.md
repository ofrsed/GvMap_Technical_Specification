# GvMap_Technical_Specification

## Оглавление

1. [Введение](#1-введение)
   - [Название проекта](#11-название-проекта)
   - [Цель проекта](#12-цель-проекта)
   - [Краткое описание функционала](#13-краткое-описание-функционала)
   - [Целевая аудитория](#14-целевая-аудитория)
2. [Описание системы](#2-описание-системы)
   - [Типы пользователей](#21-типы-пользователей)
   - [Режимы просмотра объявлений](#22-режимы-просмотра-объявлений)
   - [Регистрация и авторизация](#23-регистрация-и-авторизация)
   - [Поиск и фильтрация](#24-поиск-и-фильтрация)
   - [Взаимодействие с пользователями](#25-взаимодействие-с-пользователями)
   - [Безопасность и анти-мошенничество](#26-безопасность-и-анти-мошенничество)
   - [Платежная система](#27-платежная-система)
3. [Дизайн и пользовательский интерфейс](#3-дизайн-и-пользовательский-интерфейс)
4. [Технические требования](#4-технические-требования)
5. [Безопасность и конфиденциальность](#5-безопасность-и-конфиденциальность)
6. [Тестирование](#6-тестирование)
7. [Сроки и этапы выполнения](#7-сроки-и-этапы-выполнения)
8. [Оценка рисков](#8-оценка-рисков)
9. [Примечания](#9-примечания)


## 1. Введение
### 1.1. Название проекта: GvMap
### 1.2. Цель проекта:
Разработка платформы для обмена вещами, мебелью и животными без финансовых затрат. Сервис позволит пользователям безвозмездно отдавать ненужные предметы и находить полезные вещи для себя. Проект ориентирован на людей, которые хотят уменьшить потребление, улучшить экологию и помочь другим, передавая или получая вещи без денег.

### 1.3. Краткое описание функционала
- Размещение и поиск объявлений
- Оценка и отзывы о пользователях
- Встроенная система чатов и переговоров между Получателями и дарителями
- Проверка пользователей (авторизация, верификация)
- Фильтрация объявлений по категориям и регионам
- Система жалоб и блокировки подозрительных пользователей

### 1.4. Целевая аудитория.
Сервис предназначен для широкого круга пользователей, включая студентов, молодые семьи,экологически осознанных людей, а также тех, кто ищет способы сэкономить или избавляться от лишних вещей. 

## 2. Описание системы

### 2.1. Типы пользователей
Две роли - __Авторизованный пользователь__ и __Гость__.

#### 2.1.1 Авторизованный пользователь

- Возможность размещать объявления с подробным описанием предмета/животного, фотографии.
- просматривать контакты, указанные в чужих объявлениях и писать в чат другим пользователям.
- Функция редактирования и удаления объявлений.
  
#### 2.1.1 Гость

- просмотр объявлений (не видит контактов, не может пользоваться чатом)

### 2.2 Режимы просмотра объявлений

- __Классический каталог объявлений__ - Страница с категориями/подкатегориями и карточками объявлений (как на Ozon, Avito и п.р.)
- __Интерактивная карта__ - фишка проекта, карта позволяет оценить расстояние до объявления, что помогает избежать лишних затрат. (Например: не выгодно ехать за бесплатной мебелью в другой город)

### 2.3. Регистрация и авторизация

- Пользователь должен иметь возможность зарегистрироваться с помощью номера телефона, электронной почты или через социальные сети.
- Верификация личности с использованием дополнительных методов (через СМС).
- Поддержка двухфакторной аутентификации.

### 2.4. Поиск и фильтрация
- Поиск по ключевым словам, категориям, географическому положению.

### 2.5. Взаимодействие с пользователями
- Встроенная система сообщений и чатов.
- Возможность задавать вопросы, оставлять комментарии к объявлениям.
- Оценка пользователей после сделок с возможностью оставлять отзывы.

### 2.6. Безопасность и анти-мошенничество
- Верификация объявлений.
- Функция жалоб на подозрительных пользователей и контент.
- Автоматическая блокировка объявлений, если они не соответствуют требованиям безопасности.
- Внедрение системы «черного списка» для нарушителей.

### 2.7. Платежная система
- Полностью отсутствует.

## 3. Дизайн и пользовательский интерфейс
### 3.1. Основные принципы дизайна
- Минимализм
- Интуитивно понятное управление для всех категорий пользователей.
- Простота интерфейса.
- Адаптивный дизайн для мобильных устройств с разными разрешениями экранов.

### 3.2. Структура интерфейса
- **Главная страница:** Информация о проекте, Блок с последними объявлениями, Вопросы.
- **Объявления: Каталог** Категории/подкатегории объявлений, блок отфильтрованных объявлений.
- **Объявления: Карта** Категории/подкатегории объявлений, блок отфильтрованных объявлений.
- **Личный кабинет:** История объявлений, информация пользователя, ачивки, отзывы, настройки профиля, уведомления.
- **Страница объявления:** Подробности, фотографии, кнопка связи с продавцом, блок с инфо о пользователе.
- **Чат:** Интерактивное окно для общения между пользователями.

### 3.3. Анимации и переходы
- Плавные анимации должны быть минимальны, без излишних эффектов. Интерфейс должен быть максимально простым и удобным, без ненужных движений.
- Визуальные эффекты при добавлении и редактировании объявлений.

## 4. Технические требования
### 4.1. Платформы
- Приложение будет доступно на мобильных устройствах с операционными системами iOS (с версии 12 и выше) и Android (с версии 7.0 и выше).
- Для ПК будет доступна веб-версия, поддерживающая все современные браузеры (Chrome, Firefox, Safari, Edge).

### 4.2. Интеграции
- Система геолокации для отображения объявлений по регионам.
- Встроенная система мониторинга безопасности.

### 4.3. Производительность
- Приложение должно обеспечивать быструю загрузку страниц и объявлений.
- Низкое потребление трафика и ресурсов устройства.

### 4.4. Архитектура
- Клиент-серверная архитектура с использованием REST API для обмена данными.
- Серверная часть: масштабируемость и защита от атак.

## 5. Безопасность и конфиденциальность
- Все персональные данные пользователей должны быть защищены в соответствии с законодательством.
- Вся передаваемая информация должна быть зашифрована.
- Резервное копирование данных для предотвращения потери информации.

## 6. Тестирование
### 6.1. Виды тестирования
- **Функциональное тестирование:** Проверка работы всех функций приложения.
- **Тестирование безопасности:** Проверка уязвимостей и защита данных.
- **Тестирование производительности:** Оценка нагрузки и скорости работы.

### 6.2. Требования к тестированию
- Тестирование на реальных устройствах.
- Многоуровневое тестирование интерфейса и юзабилити.

## 7. Сроки и этапы выполнения
### 7.1. Этапы разработки
~~1. **Исследование и проектирование:** None~~
~~2. **Разработка MVP (минимально жизнеспособного продукта):** None~~
~~3. **Тестирование:** None~~
~~4. **Запуск бета-версии:** None~~
~~5. **Запуск в продакшн:** None~~

### 7.2. Ожидаемые сроки завершения проекта
~~- Общий срок реализации: None~~

## 8. Оценка рисков
### 8.1. Риски безопасности
- Мошенничество пользователей (решение: система верификации, жалобы).
- Утечка данных (решение: шифрование и защита данных).

### 8.2. Риски производительности
- Высокая нагрузка на сервер (решение: масштабируемая архитектура, CDN).
- Проблемы с работой на разных устройствах (решение: тестирование на всех платформах).

## 9. Примечания


