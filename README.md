# 🌐 MiGiTi Proxy Subscriptions

<p align="center">
  <a href="https://github.com/misha12333211-ctrl/proxy-subs/stargazers">
    <img src="https://img.shields.io/github/stars/misha12333211-ctrl/proxy-subs?style=for-the-badge&color=007EC6" alt="Stars">
  </a>
  <a href="https://github.com/misha12333211-ctrl/proxy-subs/issues">
    <img src="https://img.shields.io/github/issues/misha12333211-ctrl/proxy-subs?style=for-the-badge&color=007EC6" alt="Issues">
  </a>
  <a href="https://github.com/misha12333211-ctrl/proxy-subs/commits/main">
    <img src="https://img.shields.io/github/last-commit/misha12333211-ctrl/proxy-subs?style=for-the-badge&color=007EC6" alt="Last Commit">
  </a>
</p>

Бесплатный коллектор подписок и публичных прокси-серверов V2Ray / Xray с регулярной очисткой, фильтрацией задержки и отбором рабочих конфигов.

🔗 **Официальный сайт проекта**: [misha12333211-ctrl.github.io/MiGiTi](https://misha12333211-ctrl.github.io/MiGiTi/)

---

## 📌 О проекте

Привет! Я давно увлечён темой обхода блокировок, настройкой прокси и апгрейдом домашнего интернета. Больше года я являюсь постоянным читателем канала **Киберпортал** — именно их контент и активное сообщество вдохновили меня погрузиться во всё это с головой.

Базу подписок я собираю вручную: ищу свежие конфигурации в открытом доступе, прогоняю их через тесты и отбираю только те, которые действительно работают, держат стабильную связь и дают адекватный пинг.

---

## 🛠 Как отбираются и чистятся сервера

Каждый сервер в подписке проходит обязательную фильтрацию:

* 🔎 **Ручной отбор** — Поиск и проверка новых конфигов в профильных сообществах и Telegram-каналах.
* ⚡ **Фильтр задержки (Ping Validation)** — Нерабочие и медленные узлы отсеиваются. В список `FAST PING` попадают только серверы с задержкой до **90 мс**.
* 🧹 **Чистка дублей** — Удаление повторяющихся конфигураций и сортировка по категориям (*Whitelist*, *Fast Ping*, *Universal*, *Stealth NextGen*).

---

## ⚙️ Важно: Рекомендуемые настройки клиентов

> [!IMPORTANT]  
> Ключевую роль в обходе блокировок играет то, как именно настроен ваш клиент. После сотен тестов я подобрал оптимальные конфигурации под популярные приложения.

> [!TIP]
> **Раздельное туннелирование (Режим VPN для приложений):**  
> В настройках каждого из клиентов обязательно перейдите в раздел **«Режим VPN для приложений»** (или *Per-app proxy* / *Split tunneling*) и укажите **все российские приложения** (Госуслуги, Банки, Яндекс, VK и др.), чтобы они направлялись в обход (мимо) VPN.

### Варианты DNS-серверов (выберите один):
* `1.1.1.1`
* `77.88.8.8`
* `dns.alidns.com`
* `https://dns.astracat.ru/DNS-QUERY`

---

<details>
<summary>📱 <b>Настройка v2rayNG</b> (Скачать: <a href="https://github.com/2dust/v2rayNG/releases/tag/2.2.6">Releases</a>)</summary>

<br>

| Параметр | Значение / Настройка |
| :--- | :--- |
| **Fake DNS** | 🟢 **Обязательно включить** |
| **MTU** | `1281` |
| **DNS (Удалённый и Внутренний)** | Один из списка выше |
| **Маршрутизация** | `ipifnonmatch` |
| **Поставщик правил** | `loyalsolider` |
| **VPN для приложений** | 🟢 Настроить исключение для всех российских сервисов |

#### ✂️ Фрагментация (Fragment) — Обязательно включить:
* **Длина (Length):** `5-10`
* **Интервал (Interval):** `5-15`
* **Максимальное число пакетов (при наличии):** `20`

</details>

<details>
<summary>📱 <b>Настройка Husi</b> (Скачать: <a href="https://github.com/xchacha20-poly1305/husi/releases">Releases</a>)</summary>

<br>

| Параметр | Значение / Настройка |
| :--- | :--- |
| **Стек (TUN)** | `gvisor` |
| **MTU** | `1281` |
| **Fake DNS** | 🟢 **Включить** + Применять Fake DNS для каждого домена |
| **DNS** | Один из списка выше |
| **Маршрутизация** | `ipifnonmatch` |
| **Поставщик правил** | `loyalsolider` |
| **VPN для приложений** | 🟢 Настроить исключение для всех российских сервисов |
| **Дополнительно** | 🟢 Включить **Wakelock** |

</details>

<details>
<summary>📱 <b>Настройка Exclave</b> (Скачать: <a href="https://github.com/ExclaveNetwork/Exclave/releases">Releases</a>)</summary>

<br>

| Параметр | Значение / Настройка |
| :--- | :--- |
| **Стек** | `gvisor` |
| **MTU** | `1281` |
| **DNS** | Один из списка выше + 🟢 Включить маршрутизацию DNS |
| **Перехват & Анализ** | 🟢 Перехват DNS <br> 🟢 Анализ трафика <br> 🟢 Переопределить адрес назначения |
| **Маршрутизация** | Поставщик: `loyalsolider` \| Режим: `Глобальный` |
| **Протоколы** | 🟢 Включить «Отключить REALITY» <br> 🟢 Включить Hysteria 2 |
| **Фрагментация** | 🟢 Включить фрагментацию TLS <br> 🟢 Метод: *Фрагментация и сегментация* <br> 🟢 Включить фрагментацию для прямого |
| **VPN для приложений** | 🟢 Настроить исключение для всех российских сервисов |
| **Дополнительно** | 🟢 FakeDNS <br> 🟢 Включить **Wakelock** |

</details>

---

## 🛡️ Блокировка рекламы и аналитики (включая YouTube)

Я очень долго искал рабочий способ заблокировать рекламу в YouTube и системные трекеры. В итоге я создал собственную маршрутизацию. 

Чтобы избавиться от рекламы, создайте в вашем клиенте **новое правило маршрутизации** со значением действия **«Блокировать / Block»** и скопируйте туда следующий список доменов и регулярных выражений:

`firebaselogging.googleapis.com,play.googleapis.com,google-analytics.com,ssl.google-analytics.com,doubleclick.net,*.doubleclick.net,pubads.g.doubleclick.net,pagead2.googlesyndication.com,googleadservices.com,domain:firebaseio.com,full:firebaselogging.googleapis.com,full:play.googleapis.com,domain:google-analytics.com,domain:doubleclick.net,full:pagead2.googlesyndication.com,full:googleadservices.com,full:s.youtube.com,full:video-stats.l.google.com,domain:crashlytics.com,domain:app-measurement.com,domain:googletagservices.com,domain:googletagmanager.com,domain:s.youtube.com,domain:video-stats.l.google.com,domain:exile.e.youtube.com,domain:google-analytics.com,domain:ssl.google-analytics.com,domain:stats.g.doubleclick.net,regexp:^.*youtube.*\/ptracking$,regexp:^.*youtube.*\/stream_204$,regexp:^.*youtube.*\/gen_204$,domain:sentry.io,domain:samsung-analytics.com,domain:samsungosp.com,geosite:category-ads-all,domain:sentry.io,domain:crashlytics.com,google-analytics.com,firebaseanalytics.amazonaws.com,firebaseio.com,crashlytics.com,telemetry.google,graph.facebook.com,facebook-hardware.com,analytics.whatsapp.com,crashlogs.whatsapp.net,stat.com.telegram,app-measurement.com,samsung-analytics.com,samsungosp.com,samsungcloudplatform.com,logging.samsungdm.com,com.sec.android.app.sbrowser,com.samsung.android.messaging,com.facebook.orca,com.whatsapp,com.android.chrome,com.google.android.googlequicksearchbox,com.android.vending,com.google.android.apps.maps,connectivitycheck.gstatic.com,telemetry.google.com,google-analytics.com,ssl.google-analytics.com,analytics.google.com,firebaseio.com,firebase-settings.crashlytics.com,crashlytics.com,reports.crashlytics.com,api.crashlytics.com,play.googleapis.com,android.clients.google.com,android-context-data.googleapis.com,safebrowsing.googleapis.com,app-measurement.com,adjust.com,app.adjust.com,app.tr.adjust.com,tracking.intl.miui.com,api.sec.intl.miui.com,api.ad.intl.xiaomi.com,data.mistat.xiaomi.com,sdkconfig.ad.intl.xiaomi.com,api.omc.samsungdm.com,samsung-directory.edge.hiyaapi.com,capi.samsungcloud.com,gos-api.gos-gsp.io,dir-apis.samsungdm.com,api.gras.samsungdm.com,sspapi-prd.samsungrs.com,sdk.pushmessage.samsung.com,us-api.mcsvc.samsung.com,eu-api.mcsvc.samsung.com,ie-odc.samsungapps.com,in.appcenter.ms,query.hicloud.com,configserverdre.platform.hicloud.com,servicesupport.hicloud.com,pebed.dmevent.net,telemetry.api.swiftkey.com,esa-reg-eup.myoppo.com,ifotaeu.realmemobile.com,ifotaus.realmemobile.com,domain:bixbywelcome.samsung.com,domain:bixby.samsung.com,domain:customization.samsung.com,domain:samsungcloud.com,domain:account.samsung.com,domain:legal.samsung.com,domain:galaxyapps.samsung.com,domain:fota-cloud-dn.ospserver.net,domain:oemprd.samsungcloudsolution.com,domain:telemetry.darkness.google,domain:android.bugreport.google.com,domain:location.googleapis.com,domain:coauth.googleapis.com,domain:grandcentral.googleapis.com,domain:speech.googleapis.com,domain:appsflyer.com,domain:appflyer.com,domain:amplitude.com,domain:api.amplitude.com,domain:mixpanel.com,domain:api.mixpanel.com,domain:flurry.com,domain:data.flurry.com,domain:onesignal.com,domain:branch.io,domain:api2.branch.io,domain:bugsnag.com,domain:notify.bugsnag.com,regexp:^analytics\..*$,regexp:^telemetry\..*$,regexp:^.*metrics.*$,regexp:^.*log-stat.*$,domain:time.android.com,domain:time.google.com,domain:time.windows.com`

---

## 🔗 Ссылки на подписки

Скопируйте и вставьте нужную ссылку в ваш клиент:

### 1. Стандартные подписки (GitHub)

* ⚪ **01 MIGITI WHITELIST** *(Оптимизировано для РФ-сервисов: Яндекс, VK, Госуслуги)*:  
  `https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/1.txt`

* ⚡ **02 MIGITI FAST PING** *(Быстрые серверы с пингом до 90 мс)*:  
  `https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/2.txt`

* 🌐 **03 MIGITI UNIVERSAL** *(Сборная подписка: VLESS, VMess, Trojan, Shadowsocks)*:  
  `https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/3.txt`

* 🥷 **04 MIGITI STEALTH NEXTGEN** *(Конфигурации VLESS REALITY и UDP-протоколы)*:  
  `https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/4.txt`

---

### 2. Обновление через Яндекс Переводчик *(если GitHub заблокирован)*

> [!TIP]  
> Если GitHub блокируется вашим провайдером, используйте эти зеркала для обновления. *(Спасибо авторам репозитория [vpn-configs-for-russia](https://github.com/igareck/vpn-configs-for-russia) за лайфхак!)*

* ⚪ **01 MIGITI WHITELIST**:  
  `https://translate.yandex.ru/translate?url=https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/1.txt&lang=de-de`

* ⚡ **02 MIGITI FAST PING**:  
  `https://translate.yandex.ru/translate?url=https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/2.txt&lang=de-de`

* 🌐 **03 MIGITI UNIVERSAL**:  
  `https://translate.yandex.ru/translate?url=https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/3.txt&lang=de-de`

* 🥷 **04 MIGITI STEALTH NEXTGEN**:  
  `https://translate.yandex.ru/translate?url=https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/4.txt&lang=de-de`

---

## 💳 Поддержать проект (Donate)

Проект полностью бесплатный, но отбор и поддержка базы требуют времени. Если проект вам пригодился, буду благодарен за поддержку:

* 🟢 **Сбербанк**: [Перевести через Сбер](https://messenger.online.sberbank.ru/sl/HB0CuMt88gO20oajp)
* 🧡 **Patreon**: [Мой Patreon](https://www.patreon.com/cw/MiGiTiVlessSubscriptions/shop?sort=published_at)
* 🎁 **DonationAlerts**: [donationalerts.com/r/diagomalacco](https://www.donationalerts.com/r/diagomalacco)
* 💎 **TON Wallet**: `UQB4NY_1ula9p2YJpM0kHPEjbJOmOUK1JNwYUNu9_T2TlAbt`

---

## ⚖️ Отказ от ответственности (Disclaimer)

Данный проект является публичным **агрегатором и фильтром** конфигураций. Все прокси-серверы собираются из открытых источников в сеть Интернет. Автор проекта не владеет большей частью серверов и не несёт ответственности за их содержимое.

Если вы являетесь владельцем конкретного сервера/конфигурации и хотите, чтобы ваш узловой адрес был удалён из списков подписки — напишите на [Fageter@protonmail.com](mailto:Fageter@protonmail.com) или создайте [Issue](https://github.com/misha12333211-ctrl/proxy-subs/issues). Узел будет оперативно удалён.

---

## 📬 Обратная связь

* 📧 **Email**: `Fageter@protonmail.com`
* 💬 **GitHub Issues**: Пишите вопросы и предложения в разделе [Issues](https://github.com/misha12333211-ctrl/proxy-subs/issues).
