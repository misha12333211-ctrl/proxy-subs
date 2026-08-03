# 🌐 MiGiTi Proxy Subscriptions

<p align="center">
  <img src="https://img.shields.io/github/stars/misha12333211-ctrl/proxy-subs?style=for-the-badge&color=white" alt="Stars">
  <img src="https://img.shields.io/github/forks/misha12333211-ctrl/proxy-subs?style=for-the-badge&color=white" alt="Forks">
  <img src="https://img.shields.io/github/license/misha12333211-ctrl/proxy-subs?style=for-the-badge&color=white" alt="License">
</p>

Агрегатор и коллекция подписок публичных прокси-узлов V2Ray/Xray с ручной и автоматической фильтрацией, валидацией пинга и блокировкой рекламы, телеметрии и трекеров.

🔗 **Официальный сайт проекта**: [misha12333211-ctrl.github.io/proxy-subs](https://misha12333211-ctrl.github.io/proxy-subs/)

---

## 📌 О проекте & Вдохновение

Привет! Я увлекаюсь сетевыми технологиями, архитектурой обхода блокировок и оптимизацией VPN/Proxy уже долгое время. Более года я активно слежу за Telegram-каналом **Киберпортал** — являюсь их постоянным читателем и фанатом. Почерпнутая оттуда информация и материалы комьюнити вдохновили меня на глубокое погружение в тему прокси, правила маршрутизации и кастомные конфигурации.

Вся база подписок в этом проекте отбирается очень тщательно: я **собственными руками нахожу конфигурации и подписки на просторах интернета, лично тестирую и проверяю каждую из них на работоспособность, пинг и стабильность**.

---

## 🛠 Ручная и Автоматическая Очистка Узлов

Каждая конфигурация и подписка проходит проверку по нескольким критериям:

1. **Ручной отбор**: Поиск рабочих узлов в публичных источниках и Telegram-сообществах.
2. **Проверка пинга (Ping Validation)**: Фильтрация серверов с высокой задержкой. В список `FAST PING` попадают только узлы с задержкой менее 90 мс.
3. **Дедупликация и сортировка**: Очистка дубликатов и распределение по категории (Whitelist, Fast Ping, Universal, Stealth NextGen).

---

## 💡 Обновление подписок через Яндекс Переводчик

Полезный лайфхак для клиентов, у которых возникают проблемы с прямолинейной загрузкой подписок или блокировкой GitHub:

Вы можете прогонять и обновлять ссылки на подписки через проксирующий интерфейс Яндекс Переводчика. Для этого подставьте URL нужного `.txt` файла в следующий формат:

```text
[https://translate.yandex.ru/translate?url=ПОДПИСКА&lang=de-de](https://translate.yandex.ru/translate?url=ПОДПИСКА&lang=de-de)
```

> Выражаю благодарность репозиторию [vpn-configs-for-russia](https://github.com/igareck/vpn-configs-for-russia) за упоминание данного метода!

---

## 🛡 Правила блокировки рекламы YouTube, телеметрии и трекеров

Я глубоко разбираюсь в правилах маршрутизации и фильтрации трафика. Ниже приведен готовый список доменов, регулярных выражений и правил (geosite / domain / full / regexp), которые необходимо вносить в блокировку клиентов (v2rayN, Sing-Box, Nekobox, Happ и др.) для отключения рекламы на YouTube, блокировки системной телеметрии (Google, Samsung, Xiaomi, OPPO, Microsoft), встроенных трекеров и метрик аналитики:

```text
firebaselogging.googleapis.com,play.googleapis.com,google-analytics.com,ssl.google-analytics.com,doubleclick.net,*.doubleclick.net,pubads.g.doubleclick.net,pagead2.googlesyndication.com,googleadservices.com,domain:firebaseio.com,full:firebaselogging.googleapis.com,full:play.googleapis.com,domain:google-analytics.com,domain:doubleclick.net,full:pagead2.googlesyndication.com,full:googleadservices.com,full:s.youtube.com,full:video-stats.l.google.com,domain:crashlytics.com,domain:app-measurement.com,domain:googletagservices.com,domain:googletagmanager.com,domain:s.youtube.com,domain:video-stats.l.google.com,domain:exile.e.youtube.com,domain:google-analytics.com,domain:ssl.google-analytics.com,domain:stats.g.doubleclick.net,regexp:^.*youtube.*\/ptracking$,regexp:^.*youtube.*\/stream_204$,regexp:^.*youtube.*\/gen_204$,domain:sentry.io,domain:samsung-analytics.com,domain:samsungosp.com,geosite:category-ads-all,domain:sentry.io,domain:crashlytics.com,google-analytics.com,firebaseanalytics.amazonaws.com,firebaseio.com,crashlytics.com,telemetry.google,graph.facebook.com,facebook-hardware.com,analytics.whatsapp.com,crashlogs.whatsapp.net,stat.com.telegram,app-measurement.com,samsung-analytics.com,samsungosp.com,samsungcloudplatform.com,logging.samsungdm.com,com.sec.android.app.sbrowser,com.samsung.android.messaging,com.facebook.orca,com.whatsapp,com.android.chrome,com.google.android.googlequicksearchbox,com.android.vending,com.google.android.apps.maps,connectivitycheck.gstatic.com,telemetry.google.com,google-analytics.com,ssl.google-analytics.com,analytics.google.com,firebaseio.com,firebase-settings.crashlytics.com,crashlytics.com,reports.crashlytics.com,api.crashlytics.com,play.googleapis.com,android.clients.google.com,android-context-data.googleapis.com,safebrowsing.googleapis.com,app-measurement.com,adjust.com,app.adjust.com,app.tr.adjust.com,tracking.intl.miui.com,api.sec.intl.miui.com,api.ad.intl.xiaomi.com,data.mistat.xiaomi.com,sdkconfig.ad.intl.xiaomi.com,api.omc.samsungdm.com,samsung-directory.edge.hiyaapi.com,capi.samsungcloud.com,gos-api.gos-gsp.io,dir-apis.samsungdm.com,api.gras.samsungdm.com,sspapi-prd.samsungrs.com,sdk.pushmessage.samsung.com,us-api.mcsvc.samsung.com,eu-api.mcsvc.samsung.com,ie-odc.samsungapps.com,in.appcenter.ms,query.hicloud.com,configserverdre.platform.hicloud.com,servicesupport.hicloud.com,pebed.dmevent.net,telemetry.api.swiftkey.com,esa-reg-eup.myoppo.com,ifotaeu.realmemobile.com,ifotaus.realmemobile.com,domain:bixbywelcome.samsung.com,domain:bixby.samsung.com,domain:customization.samsung.com,domain:samsungcloud.com,domain:account.samsung.com,domain:legal.samsung.com,domain:galaxyapps.samsung.com,domain:fota-cloud-dn.ospserver.net,domain:oemprd.samsungcloudsolution.com,domain:telemetry.darkness.google,domain:android.bugreport.google.com,domain:location.googleapis.com,domain:coauth.googleapis.com,domain:grandcentral.googleapis.com,domain:speech.googleapis.com,domain:appsflyer.com,domain:appflyer.com,domain:amplitude.com,domain:api.amplitude.com,domain:mixpanel.com,domain:api.mixpanel.com,domain:flurry.com,domain:data.flurry.com,domain:onesignal.com,domain:branch.io,domain:api2.branch.io,domain:bugsnag.com,domain:notify.bugsnag.com,regexp:^analytics\..*$,regexp:^telemetry\..*$,regexp:^.*metrics.*$,regexp:^.*log-stat.*$,domain:time.android.com,domain:time.google.com,domain:time.windows.com.
```

---

## 🔗 Готовые Подписки

Ссылки для вставки в ваши клиенты V2Ray / Xray:

| № | Название | Описание | Ссылка на подписку |
|---|---|---|---|
| **01** | **MIGITI WHITELIST** | Оптимизировано под домены и сервисы РФ (Яндекс, VK, ГосУслуги) | [`1.txt`](https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/1.txt) |
| **02** | **MIGITI FAST PING** | Быстрые узлы с задержкой менее 90 мс для игр и стриминга | [`2.txt`](https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/2.txt) |
| **03** | **MIGITI UNIVERSAL** | Универсальный набор протоколов (VLESS, VMess, Trojan, Shadowsocks) | [`3.txt`](https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/3.txt) |
| **04** | **MIGITI STEALTH NEXTGEN** | VLESS REALITY и высокоскоростные UDP-протоколы | [`4.txt`](https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/4.txt) |

---

## 💳 Поддержать проект (Donate)

Проект бесплатный, однако ручной подбор, проверка узлов и поддержка сервиса требуют ресурсов. Буду рад вашей поддержке:

* 🟢 **Сбербанк**: [Перевести через Сбер](https://messenger.online.sberbank.ru/sl/HB0CuMt88gO20oajp)
* 💎 **TON Wallet**: `UQB4NY_1ula9p2YJpM0kHPEjbJOmOUK1JNwYUNu9_T2TlAbt`
* 🎁 **DonationAlerts**: [donationalerts.com/r/diagomalacco](https://www.donationalerts.com/r/diagomalacco)

---

## 📬 Контакты и Обратная связь

* **Email**: `Fageter@proronmail.com`
* **GitHub Issues**: Оставляйте отзывы и предложения в разделе Issues текущего репозитория.
