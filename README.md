# 🌐 MiGiTi Proxy Subscriptions

<p align="center">
  <a href="https://github.com/misha12333211-ctrl/proxy-subs/stargazers">
    <img src="https://img.shields.io/github/stars/misha12333211-ctrl/proxy-subs?style=flat&label=stars&color=blue" alt="Stars">
  </a>
  <a href="https://github.com/misha12333211-ctrl/proxy-subs">
    <img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fmisha12333211-ctrl%2Fproxy-subs&count_bg=%23007EC6&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visitors&edge_flat=false" alt="Visitors">
  </a>
  <a href="https://github.com/misha12333211-ctrl/proxy-subs/issues">
    <img src="https://img.shields.io/github/issues/misha12333211-ctrl/proxy-subs?style=flat&label=issues&color=blue" alt="Issues">
  </a>
  <br>
  <a href="https://github.com/misha12333211-ctrl/proxy-subs/commits/main">
    <img src="https://img.shields.io/github/last-commit/misha12333211-ctrl/proxy-subs?style=flat&label=last%20commit&color=blue" alt="Last Commit">
  </a>
  <img src="https://img.shields.io/badge/Open%20Source-%F0%9F%A4%8D-brightgreen" alt="Open Source">
  <br>
  <a href="mailto:Fageter@proronmail.com">
    <img src="https://img.shields.io/badge/Email-Fageter%40proronmail.com-007EC6?style=flat&logo=gmail&logoColor=white" alt="Email">
  </a>
</p>

<p align="center">
  <a href="https://www.donationalerts.com/r/diagomalacco">
    <img src="https://img.shields.io/badge/SUPPORT%20ME%20ON-DONATIONALERTS-FF5E36?style=for-the-badge&logo=donationalerts&logoColor=white" alt="Donate">
  </a>
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
firebaselogging.googleapis.com,play.googleapis.com,google-analytics.com,ssl.google-analytics.com,doubleclick.net,*.doubleclick.net,pubads.g.doubleclick.net,pagead2.googlesyndication.com,googleadservices.com,domain:firebaseio.com,full:firebaselogging.googleapis.com,full:play.googleapis.com,domain:google-analytics.com,domain:doubleclick.net,full:pagead2.googlesyndication.com,full:googleadservices.com,full:s.youtube.com,full:video-stats.l.google.com,domain:crashlytics.com,domain:app-measurement.com,domain:googletagservices.com,domain:googletagmanager.com,domain:s.youtube.com,domain:video-stats.l.google.com,domain:exile.e.youtube.com,domain:google-analytics.com,domain:ssl.google-analytics.com,domain:stats.g.doubleclick.net,regexp:^.*youtube.*\/ptracking$,regexp:^.*youtube.*\/stream_204$,regexp:^.*youtube.*\/gen_204$,domain:sentry.io,domain:samsung-analytics.com,domain:samsungosp.com,geosite:category-ads-all,domain:sentry.io,domain:crashlytics.com,google-analytics.com,firebaseanalytics.amazonaws.com,firebaseio.com,crashlytics.com,telemetry.google,graph.facebook.com,facebook-hardware.com,analytics.whatsapp.com,crashlogs.whatsapp.net,stat.com.telegram,app-measurement.com,samsung-analytics.com,samsungosp.com,samsungcloudplatform.com,logging.samsungdm.com,com.sec.android.app.sbrowser,com.samsung.android.messaging,com.facebook.orca,com.whatsapp,com.android.chrome,com.google.android.googlequicksearchbox,com.android.vending,com.google.android.apps.maps,connectivitycheck.gstatic.com,telemetry.google.com,google-analytics.com,ssl.google-analytics.com,analytics.google.com,firebaseio.com,firebase-settings.crashlytics.com,crashlytics.com,reports.crashlytics.com,api.crashlytics.com,play.googleapis.com,android.clients.google.com,android-context-data.googleapis.com,safebrowsing.googleapis.com,app-measurement.com,adjust.com,app.adjust.com,app.tr.adjust.com,tracking.intl.miui.com,api.sec.intl.miui.com,api.ad.intl.xiaomi.com,data.mistat.xiaomi.com,sdkconfig.ad.intl.xiaomi.com,api.omc.samsungdm.com,samsung-directory.edge.hiyaapi.com,capi.samsungcloud.com,gos-api.gos-gsp.io,dir-apis.samsungdm.com,api.gras.samsungdm.com,sspapi-prd.samsungrs.com,sdk.pushmessage.samsung.com,us-api.mcsvc.samsung.com,eu-api.mcsvc.samsung.com,ie-odc.samsungapps.com,in.appcenter.ms,query.hicloud.com,configserverdre.platform.hicloud.com,servicesupport.hicloud.com,pebed.dmevent.net,telemetry.api.swiftkey.com,esa-reg-eup.myoppo.com,ifotaeu.realmemobile.com,ifotaus.realmemobile.com,domain:bixbywelcome.samsung.com,domain:bixby.samsung.com,domain:customization.samsung.com,domain:samsungcloud.com,domain:account.samsung.com,domain:legal.samsung.com,domain:galaxyapps.samsung.com,domain:fota-cloud-dn.os
