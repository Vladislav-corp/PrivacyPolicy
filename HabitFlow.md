# HabitFlow — Privacy Policy

**Last updated:** 2026-05-13

## Overview / Обзор

HabitFlow — iOS приложение для отслеживания привычек. Все данные хранятся локально на устройстве через SwiftData. У HabitFlow нет серверов, аккаунтов и облачной синхронизации.

HabitFlow is an iOS habit tracker. All data is stored locally on your device via SwiftData. HabitFlow has no servers, accounts, or cloud sync.

## What we store / Что мы храним

Только то, что вы сами создаёте в приложении: названия привычек, расписания, отметки выполнения, заметки. Данные живут в локальной SwiftData-базе и shared App Group container для синхронизации с виджетом.

Only what you create in the app: habit names, schedules, completion marks, notes. Data lives in a local SwiftData store and a shared App Group container for widget synchronization.

## Data never leaves your device / Данные не покидают устройство

HabitFlow не передаёт никакие данные на серверы — у HabitFlow нет серверов. Нет аккаунтов, нет облачного бэкапа, нет third-party аналитики (Firebase, Amplitude, Mixpanel, Sentry и т.п.).

HabitFlow does not transmit any data to servers — HabitFlow has no servers. No accounts, no cloud backup, no third-party analytics (Firebase, Amplitude, Mixpanel, Sentry, etc.).

## Notifications / Уведомления

HabitFlow использует local notifications (через `UNUserNotificationCenter`) для напоминаний о привычках. Push notifications через сервер НЕ используются. Разрешение запрашивается только когда вы включаете напоминание в привычке. Отозвать можно через Settings → Notifications → HabitFlow.

HabitFlow uses local notifications (via `UNUserNotificationCenter`) for habit reminders. No server-driven push notifications are used. Permission is requested only when you enable a reminder on a habit. You can revoke it via Settings → Notifications → HabitFlow.

## Required Reason APIs / Декларация API

Согласно требованиям Apple, HabitFlow декларирует использование:

- `UserDefaults` (reason `CA92.1`) — настройки приложения и состояние виджета.
- File timestamp APIs (reason `C617.1`) — стандартные операции SwiftData с локальным хранилищем.

Per Apple's Required Reason API rules, HabitFlow declares:

- `UserDefaults` (reason `CA92.1`) — app settings and widget state.
- File timestamp APIs (reason `C617.1`) — standard SwiftData operations on local storage.

## Tracking / Трекинг

HabitFlow не отслеживает вас между приложениями и сайтами. `NSPrivacyTracking = false`, `NSPrivacyTrackingDomains` пустой.

HabitFlow does not track you across apps and websites. `NSPrivacyTracking = false`, `NSPrivacyTrackingDomains` empty.

## Subscriptions and purchases / Подписки и покупки

В текущей версии HabitFlow полностью бесплатен и не содержит in-app purchases или подписок.

This version of HabitFlow is fully free and contains no in-app purchases or subscriptions.

## Children / Дети

HabitFlow не предназначен для детей младше 13 лет.

HabitFlow is not intended for children under 13.

## Changes / Изменения

При существенных изменениях этой политики мы обновим дату вверху файла и сообщим в App Store update notes.

For material changes to this policy, we will update the date at the top and announce it in App Store update notes.

## Contact / Контакты

Email: vrnrelax@gmail.com
Developer: Individual Entrepreneur Vladislav Kolupaev
