# Habio – Privacy Policy

**Last updated:** 2026-09-23

## Overview / Обзор

Habio – iOS приложение для отслеживания привычек. Ваши привычки и отметки хранятся локально на устройстве через SwiftData. У Habio нет своих серверов, аккаунтов и облачной синхронизации. Для улучшения приложения используется обезличенная аналитика TelemetryDeck, подробности ниже.

Habio is an iOS habit tracker. Your habits and check-ins are stored locally on your device via SwiftData. Habio has no servers of its own, no accounts, and no cloud sync. To improve the app, Habio uses anonymized analytics by TelemetryDeck, described below.

## What we store / Что мы храним

Только то, что вы сами создаёте в приложении: названия привычек, расписания, отметки выполнения, заметки. Данные живут в локальной SwiftData-базе и shared App Group container для синхронизации с виджетом.

Only what you create in the app: habit names, schedules, completion marks, notes. Data lives in a local SwiftData store and a shared App Group container for widget synchronization.

## Your habits stay on your device / Ваши привычки остаются на устройстве

Названия привычек, расписания, отметки выполнения и заметки никуда не передаются. Нет аккаунтов и облачного бэкапа.

Habit names, schedules, check-ins, and notes are never transmitted. There are no accounts and no cloud backup.

## Analytics / Аналитика

Habio использует TelemetryDeck (TelemetryDeck GmbH, Германия), privacy-first сервис аналитики, чтобы понимать, как используется приложение и экран Habio Premium. Передаются только обезличенные события:

- запуск приложения и длительность сессии;
- показ экрана Premium и откуда он открыт;
- нажатие на кнопку покупки и выбранный план;
- покупка, ожидающая подтверждения (например, «Попросить купить»);
- факт покупки или начала пробного периода: план, цена, валюта и страна магазина;
- переход с пробного периода на платную подписку.

Вместе с событиями TelemetryDeck получает технические данные: версию приложения и iOS, модель устройства и параметры экрана, язык, регион и часовой пояс, светлую или тёмную тему, настройки специальных возможностей (жирный шрифт, размер текста, уменьшение движения и подобные), время события (час, день недели), ориентацию экрана, способ установки (App Store или TestFlight), дату первого запуска, обобщённую статистику использования (число и длительность сессий, число дней с запусками), а также идентификатор устройства, который хешируется (SHA-256) на устройстве до отправки. Эти данные не связаны с вашей личностью, не используются для рекламы и трекинга и не передаются третьим лицам. Содержимое ваших привычек в аналитику не попадает.

Habio uses TelemetryDeck (TelemetryDeck GmbH, Germany), a privacy-first analytics service, to understand how the app and the Habio Premium screen are used. Only anonymized events are sent:

- the app was launched, and how long the session lasted;
- the Premium screen was shown, and where it was opened from;
- the purchase button was tapped, and which plan was selected;
- a purchase is pending approval (for example, Ask to Buy);
- a purchase or free trial started: plan, price, currency, and store country;
- a free trial converted to a paid subscription.

Along with these events TelemetryDeck receives technical data: app and iOS version, device model and screen parameters, language, region and time zone, light or dark appearance, accessibility settings (bold text, text size, reduce motion, and similar), event time (hour, day of week), screen orientation, install source (App Store or TestFlight), first launch date, aggregated usage statistics (number and length of sessions, number of days with launches), and a device identifier that is hashed (SHA-256) on the device before it is sent. This data is not linked to your identity, is not used for advertising or tracking, and is not shared with third parties. The content of your habits is never included in analytics.

## Notifications / Уведомления

Habio использует local notifications (через `UNUserNotificationCenter`) для напоминаний о привычках. Push notifications через сервер НЕ используются. Разрешение запрашивается только когда вы включаете напоминание в привычке. Отозвать можно через Settings → Notifications → Habio.

Habio uses local notifications (via `UNUserNotificationCenter`) for habit reminders. No server-driven push notifications are used. Permission is requested only when you enable a reminder on a habit. You can revoke it via Settings → Notifications → Habio.

## Required Reason APIs / Декларация API

Согласно требованиям Apple, Habio декларирует использование:

- `UserDefaults` (reason `CA92.1`) – настройки приложения и состояние виджета.
- File timestamp APIs (reason `C617.1`) – стандартные операции SwiftData с локальным хранилищем.

Per Apple's Required Reason API rules, Habio declares:

- `UserDefaults` (reason `CA92.1`) – app settings and widget state.
- File timestamp APIs (reason `C617.1`) – standard SwiftData operations on local storage.

## Tracking / Трекинг

Habio не отслеживает вас между приложениями и сайтами. `NSPrivacyTracking = false`, `NSPrivacyTrackingDomains` пустой.

Habio does not track you across apps and websites. `NSPrivacyTracking = false`, `NSPrivacyTrackingDomains` empty.

## Subscriptions and purchases / Подписки и покупки

Habio предлагает платный уровень Habio Premium: автопродлеваемые подписки (месячная и годовая) и разовую покупку lifetime. Все платежи обрабатывает Apple через StoreKit. Habio не получает и не хранит платёжные данные: ни номера карт, ни адреса, ни имя владельца. Приложение видит только факт наличия активной покупки. Сведения о совершённой покупке (план, цена, валюта, страна) обезличенно передаются в аналитику, см. раздел «Аналитика».

Habio offers a paid tier, Habio Premium: auto-renewable subscriptions (monthly and yearly) and a one-time lifetime purchase. All payments are processed by Apple via StoreKit. Habio neither receives nor stores payment data: no card numbers, no addresses, no cardholder name. The app only sees whether an active purchase exists. Details of a completed purchase (plan, price, currency, country) are sent to analytics anonymously, see the Analytics section.

## Children / Дети

Habio не предназначен для детей младше 13 лет.

Habio is not intended for children under 13.

## Changes / Изменения

При существенных изменениях этой политики мы обновим дату вверху файла и сообщим в App Store update notes.

For material changes to this policy, we will update the date at the top and announce it in App Store update notes.

## Contact / Контакты

Email: vrnrelax@gmail.com
Developer: Individual Entrepreneur Vladislav Kolupaev
