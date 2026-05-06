# Vitals — Privacy Policy

**Last updated:** 2026-04-29

## Overview / Обзор

Vitals — iOS приложение, превращающее данные Apple Health в один понятный score 0–100. Все вычисления и хранение данных происходят локально на устройстве.

Vitals is an iOS app that turns Apple Health data into a single 0–100 health score. All computation and storage happens locally on your device.

## Data we read / Какие данные читаем

Только метрики, которые вы явно разрешили в системном диалоге Apple Health: пульс, HRV, шаги, активные калории, сон, кислород в крови, дыхание и другие. Без вашего разрешения Vitals не читает ничего.

Only metrics you explicitly grant via the system Apple Health dialog: heart rate, HRV, steps, active energy, sleep, blood oxygen, respiration, and others. Without your permission Vitals reads nothing.

## No data leaves your device / Данные не покидают устройство

Vitals не передаёт health-данные на серверы — у Vitals нет серверов. Корреляции, инсайты, аномалии и weekly digest вычисляются on-device с использованием Pearson correlation и z-score статистики.

Vitals does not send health data to servers — Vitals has no servers. Correlations, insights, anomalies, and weekly digests are computed on-device using Pearson correlation and z-score statistics.

Кэш истории метрик хранится в App Support directory приложения. Состояние подписки хранится в `UserDefaults` и в shared App Group container для синхронизации с виджетом.

Metric history cache is stored in the app's App Support directory. Subscription state is kept in `UserDefaults` and a shared App Group container for widget synchronization.

## Apple Health integration / Интеграция с Apple Health

Vitals только читает из Apple Health. Vitals **не пишет** в Apple Health. В любой момент вы можете отозвать разрешения через Settings → Privacy & Security → Health → Vitals.

Vitals only reads from Apple Health. Vitals **does not write** to Apple Health. You can revoke permissions any time via Settings → Privacy & Security → Health → Vitals.

## Subscriptions and In-App Purchases / Подписки и покупки

Vitals Premium предлагается через auto-renewable subscriptions:

- **Monthly:** 399 ₽
- **Yearly:** 2 490 ₽ (включая 7 дней бесплатного триала)
- **Lifetime:** 6 990 ₽ (одноразовая покупка)

Подписки управляются через ваш Apple ID. Отмена в Settings → Apple ID → Subscriptions. Restore через Settings экран в приложении или App Store.

Vitals Premium is offered via auto-renewable subscriptions:

- **Monthly:** $4.99
- **Yearly:** $29.99 (includes 7-day free trial)
- **Lifetime:** $79.99 (one-time purchase)

Subscriptions are managed through your Apple ID. Cancel via Settings → Apple ID → Subscriptions. Restore via Settings in the app or App Store.

## Analytics / Аналитика

В текущей версии Vitals использует только локальное логирование (console output для разработки). Никакие third-party аналитические SDK (Firebase, Amplitude, Mixpanel и т.д.) НЕ интегрированы.

Vitals currently uses only local logging (console output for development). No third-party analytics SDKs (Firebase, Amplitude, Mixpanel, etc.) are integrated.

Если в будущем будет интегрирован analytics-провайдер — эта политика будет обновлена и вы получите уведомление в приложении.

If an analytics provider is integrated in a future version, this policy will be updated and you will be notified in-app.

## Notifications / Уведомления

Vitals использует local notifications (через `UNUserNotificationCenter`) для еженедельного отчёта (по воскресеньям, если включено в Settings). Push notifications через сервер НЕ используются.

Vitals uses local notifications (via `UNUserNotificationCenter`) for the weekly digest (Sundays, if enabled in Settings). No server-driven push notifications are used.

## Children / Дети

Vitals не предназначен для детей младше 13 лет.

Vitals is not intended for children under 13.

## Changes / Изменения

При существенных изменениях этой политики мы обновим дату вверху файла и уведомим в App Store update notes.

For material changes to this policy, we will update the date at the top and notify via App Store update notes.

## Contact / Контакты

Email: vrnrelax@gmail.com
Developer: Individual Entrepreneur Vladislav Kolupaev
