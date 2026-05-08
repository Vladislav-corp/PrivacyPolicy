# Cleanbook — Privacy Policy

**Last updated:** 2026-05-08

## Overview / Обзор

Cleanbook — iOS приложение для очистки и дедупликации контактной книги. Все операции выполняются локально на устройстве. Контакты не покидают ваш iPhone.

Cleanbook is an iOS app for cleaning up and deduplicating your contacts. All operations run locally on your device. Contacts never leave your iPhone.

## Data we read / Какие данные читаем

Только ваши контакты из системной адресной книги iOS, после явного разрешения через системный диалог Apple Contacts. Без вашего разрешения Cleanbook не читает ничего.

Only your contacts from the iOS system address book, after you explicitly grant access via the system Apple Contacts dialog. Without your permission Cleanbook reads nothing.

## No data leaves your device / Данные не покидают устройство

Cleanbook не передаёт контакты на серверы — у Cleanbook нет серверов. Поиск дубликатов, sweep-сессии и работа с корзиной выполняются on-device.

Cleanbook does not send contacts to any server — Cleanbook has no servers. Duplicate detection, sweep sessions, and trash operations are computed on-device.

Удалённые в sweep-сессии контакты не пропадают сразу: они архивируются как vCard в локальной базе SwiftData (корзина) на устройстве, и их можно восстановить в течение времени удержания. После TTL запись из корзины удаляется автоматически.

Contacts deleted in a sweep session don't disappear immediately: they are archived as vCards in a local SwiftData database (trash) on the device, and can be restored during the retention period. After TTL the trash entry is purged automatically.

## Apple Contacts integration / Интеграция с Apple Contacts

Cleanbook читает, удаляет и восстанавливает контакты в системной адресной книге через `CNContactStore`. Все операции выполняются с вашим явным согласием. В любой момент вы можете отозвать разрешение через Settings → Privacy & Security → Contacts → Cleanbook.

Cleanbook reads, deletes, and restores contacts in the system address book via `CNContactStore`. All operations require your explicit consent. You can revoke permission any time via Settings → Privacy & Security → Contacts → Cleanbook.

## Storage / Хранение

- Контакты, помеченные на удаление, архивируются как vCard в локальной SwiftData-базе (корзина) и удаляются после истечения TTL.
- White-list одобренных контактов («Approved») и список «отклонённых дублей» хранятся в локальной SwiftData-базе.
- Настройки приложения (тема, состояние онбординга, активная вкладка) хранятся в `UserDefaults`.

Все данные привязаны к контейнеру приложения и удаляются при удалении приложения.

- Contacts marked for deletion are archived as vCard in a local SwiftData database (trash) and purged after TTL.
- Approved contacts white-list and dismissed duplicates list are stored in a local SwiftData database.
- App preferences (theme, onboarding state, active tab) are stored in `UserDefaults`.

All data is scoped to the app container and removed when you uninstall the app.

## Subscriptions and In-App Purchases / Подписки и покупки

Cleanbook предлагает встроенную покупку Pro, обрабатываемую Apple StoreKit. Cleanbook не получает и не хранит платёжные данные — они обрабатываются Apple. Cleanbook получает только статус активной покупки (entitlement) от Apple StoreKit on-device. Платёжная информация подчиняется Apple Privacy Policy.

Cleanbook offers an in-app Pro purchase processed by Apple StoreKit. Cleanbook does not receive or store payment information — it is handled by Apple. Cleanbook only receives the active entitlement status from Apple StoreKit on-device. Payment data is governed by Apple's Privacy Policy.

## Analytics / Аналитика

Cleanbook не интегрирует никакие third-party аналитические SDK (Firebase, Amplitude, Mixpanel и т.п.). Crash reporting и event tracking не используются. App Tracking Transparency (ATT) не запрашивается, так как ничего не отслеживается.

Cleanbook does not integrate any third-party analytics SDKs (Firebase, Amplitude, Mixpanel, etc.). No crash reporting or event tracking is used. App Tracking Transparency (ATT) is not requested because nothing is tracked.

## Notifications / Уведомления

Cleanbook не отправляет push-уведомления и не использует local notifications.

Cleanbook does not send push notifications and does not use local notifications.

## Children / Дети

Cleanbook не предназначен для детей младше 13 лет. Мы сознательно не собираем персональные данные детей младше 13 лет.

Cleanbook is not directed to children under 13. We do not knowingly collect personal information from children under 13.

## Changes / Изменения

При существенных изменениях этой политики мы обновим дату вверху файла и уведомим в App Store update notes.

For material changes to this policy, we will update the date at the top and notify via App Store update notes.

## Contact / Контакты

Email: [vrnrelax@gmail.com](mailto:vrnrelax@gmail.com)
Developer: Individual Entrepreneur Vladislav Kolupaev
