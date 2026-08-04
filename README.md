<div align="center">

  <img src="https://user-images.githubusercontent.com/74038190/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif" width="600" alt="Header Animation"/>

  # 🌐 MiGiTi Proxy Subscriptions

  <p align="center">
    <a href="https://github.com/misha12333211-ctrl/proxy-subs/stargazers">
      <img src="https://img.shields.io/github/stars/misha12333211-ctrl/proxy-subs?style=for-the-badge&color=007EC6&logo=github" alt="Stars">
    </a>
    <a href="https://github.com/misha12333211-ctrl/proxy-subs/commits/main">
      <img src="https://img.shields.io/github/last-commit/misha12333211-ctrl/proxy-subs?style=for-the-badge&color=007EC6&logo=git" alt="Last Commit">
    </a>
    <a href="https://github.com/misha12333211-ctrl/proxy-subs">
      <img src="https://visitor-badge.laobi.icu/badge?page_id=misha12333211-ctrl.proxy-subs&left_text=Visitors&left_color=555555&right_color=007EC6&style=for-the-badge" alt="Visitors Count">
    </a>
  </p>

  <p align="center">
    <b>Автоматизированный агрегатор публичных конфигураций V2Ray / Xray с проверкой доступности и фильтрацией пинга.</b>
  </p>

  <p align="center">
    🔗 <a href="https://misha12333211-ctrl.github.io/MiGiTi/"><b>Перейти на официальный сайт проекта</b></a>
  </p>

</div>

<img src="https://user-images.githubusercontent.com/74038190/212284115-f47cd8ff-2ffb-4b04-b5bf-4d1c14c0247f.gif" width="100%" />

## 📌 О проекте

Привет! Проект создан для увлеченных сетевыми технологиями пользователей, оптимизации сетевого трафика и настройки гибкой маршрутизации домашнего интернета.

База конфигураций формируется из открытых источников: данные автоматически и вручную агрегируются, проходят валидацию по доступности и фильтруются по задержке отклика для обеспечения максимальной стабильности соединения.

> [!NOTE]
> **🚀 Проект активно развивается!**  
> Сейчас сервисы работают как **агрегатор и фильтр публичных узлов**. В дальнейшем планируется расширение инфраструктуры и добавление новых высокоскоростных локаций при поддержке сообщества.

<img src="https://user-images.githubusercontent.com/74038190/212284115-f47cd8ff-2ffb-4b04-b5bf-4d1c14c0247f.gif" width="100%" />

## 🔗 Ссылки на подписки

Скопируйте нужную ссылку и вставьте в ваш клиент:

### 1. Основные подписки

⚪ **01 MIGITI WHITELIST** *(Прямая маршрутизация для локальных сервисов: Яндекс, VK, Госуслуги)*  
`https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/1.txt`

⚡ **02 MIGITI FAST PING** *(Оптимизированные узлы с низкой задержкой)*  
`https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/2.txt`

🌐 **03 MIGITI UNIVERSAL** *(Универсальный набор: VLESS, VMess, Trojan, Shadowsocks)*  
`https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/3.txt`

🥷 **04 MIGITI STEALTH NEXTGEN** *(Конфигурации VLESS REALITY и современные UDP-протоколы)*  
`https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/4.txt`

---

### 2. Альтернативные зеркала

> [!TIP]  
> Если основные ссылки недоступны у вашего провайдера, используйте резервные зеркала.

<details>
<summary><b>📋 Развернуть список альтернативных зеркал</b></summary>

<br>

⚪ **01 MIGITI WHITELIST**  
`https://translate.yandex.ru/translate?url=https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/1.txt&lang=de-de`

⚡ **02 MIGITI FAST PING**  
`https://translate.yandex.ru/translate?url=https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/2.txt&lang=de-de`

🌐 **03 MIGITI UNIVERSAL**  
`https://translate.yandex.ru/translate?url=https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/3.txt&lang=de-de`

🥷 **04 MIGITI STEALTH NEXTGEN**  
`https://translate.yandex.ru/translate?url=https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/4.txt&lang=de-de`

</details>

<img src="https://user-images.githubusercontent.com/74038190/212284115-f47cd8ff-2ffb-4b04-b5bf-4d1c14c0247f.gif" width="100%" />

## 🛠 Как отбираются и чистятся серверы

Каждый сервер в подписке проходит обязательную обработку:

* 🔎 **Агрегация** — Сбор данных из публичных Telegram-каналов и Open-Source репозиториев.
* ⚡ **Ping Validation** — Тестирование RTT-задержки и автоматическое отсеивание недоступных серверов.
* 🧹 **Дедупликация** — Автоматическая очистка повторов по ключам и IP-адресам.
* ⚪ **Валидация SNI** — Проверка корректности работы TLS/SNI заголовков.

<img src="https://user-images.githubusercontent.com/74038190/212284115-f47cd8ff-2ffb-4b04-b5bf-4d1c14c0247f.gif" width="100%" />

## ⚙️ Настройки клиентов

> [!IMPORTANT]  
> Для корректной работы и правильного распределения трафика рекомендуется настроить исключения в вашем клиенте.

> [!TIP]
> **Раздельное туннелирование (Split Tunneling / Per-app proxy):**  
> В настройках клиента перейдите в раздел **«Режим VPN для приложений»** и добавьте локальные сервисы (Госуслуги, Банки, Маркетплейсы), чтобы пускать их напрямую мимо туннеля.

### Рекомендуемые DNS-серверы:
* `1.1.1.1`
* `77.88.8.8`
* `dns.alidns.com`
* `https://dns.astracat.ru/DNS-QUERY`

---

<details>
<summary>📱 <b>v2rayNG</b> — [<a href="https://github.com/2dust/v2rayNG/releases/tag/2.2.6">Скачать Releases</a>]</summary>

<br>

| Параметр | Значение / Настройка |
| :--- | :--- |
| **Fake DNS** | 🟢 **Включить** |
| **MTU** | `1281` |
| **DNS (Удалённый и Внутренний)** | Один из списка выше |
| **Маршрутизация** | `ipifnonmatch` |
| **Поставщик правил** | `loyalsolider` |
| **Исключения для приложений** | 🟢 Настроить исключения для локальных сервисов |

#### ✂️ Фрагментация (Fragment):
* **Длина (Length):** `5-10`
* **Интервал (Interval):** `5-15`
* **Максимальное число пакетов:** `20`

</details>

<details>
<summary>📱 <b>Husi</b> — [<a href="https://github.com/xchacha20-poly1305/husi/releases">Скачать Releases</a>]</summary>

<br>

| Параметр | Значение / Настройка |
| :--- | :--- |
| **Стек (TUN)** | `gvisor` |
| **MTU** | `1281` |
| **Fake DNS** | 🟢 **Включить** + Применять для каждого домена |
| **DNS** | Один из списка выше |
| **Маршрутизация** | `ipifnonmatch` |
| **Поставщик правил** | `loyalsolider` |
| **Исключения для приложений** | 🟢 Настроить исключение для локальных сервисов |
| **Дополнительно** | 🟢 Включить **Wakelock** |

</details>

<details>
<summary>📱 <b>Exclave</b> — [<a href="https://github.com/ExclaveNetwork/Exclave/releases">Скачать Releases</a>]</summary>

<br>

| Параметр | Значение / Настройка |
| :--- | :--- |
| **Стек** | `gvisor` |
| **MTU** | `1281` |
| **DNS** | Один из списка выше + 🟢 Включить маршрутизацию DNS |
| **Перехват & Анализ** | 🟢 Перехват DNS <br> 🟢 Анализ трафика <br> 🟢 Переопределить адрес назначения |
| **Маршрутизация** | Поставщик: `loyalsolider` \| Режим: `Глобальный` |
| **Протоколы** | 🟢 Включить «Отключить REALITY» <br> 🟢 Включить Hysteria 2 |
| **Фрагментация** | 🟢 Включить фрагментацию TLS <br> 🟢 Метод: *Фрагментация и сегментация* |
| **Исключения для приложений** | 🟢 Настроить исключение для локальных сервисов |
| **Дополнительно** | 🟢 FakeDNS <br> 🟢 Включить **Wakelock** |

</details>

<img src="https://user-images.githubusercontent.com/74038190/212284115-f47cd8ff-2ffb-4b04-b5bf-4d1c14c0247f.gif" width="100%" />

## 🛡️ Блокировка рекламы и телеметрии

Для фильтрации рекламных доменов и аналитических трекеров создайте новое правило в вашем клиенте с типом действия **«Блокировать / Block»**.

<details>
<summary><b>📋 Показать полный список правил и доменов</b></summary>

<br>

`firebaselogging.googleapis.com,play.googleapis.com,google-analytics.com,ssl.google-analytics.com,doubleclick.net,*.doubleclick.net,pubads.g.doubleclick.net,pagead2.googlesyndication.com,googleadservices.com,domain:firebaseio.com,full:firebaselogging.googleapis.com,full:play.googleapis.com,domain:google-analytics.com,domain:doubleclick.net,full:pagead2.googlesyndication.com,full:googleadservices.com,full:s.youtube.com,full:video-stats.l.google.com,domain:crashlytics.com,domain:app-measurement.com,domain:googletagservices.com,domain:googletagmanager.com,domain:s.youtube.com,domain:video-stats.l.google.com,domain:exile.e.youtube.com,domain:google-analytics.com,domain:ssl.google-analytics.com,domain:stats.g.doubleclick.net,regexp:^.*youtube.*\/ptracking$,regexp:^.*youtube.*\/stream_204$,regexp:^.*youtube.*\/gen_204$,domain:sentry.io,domain:samsung-analytics.com,domain:samsungosp.com,geosite:category-ads-all,domain:sentry.io,domain:crashlytics.com,google-analytics.com,firebaseanalytics.amazonaws.com,firebaseio.com,crashlytics.com,telemetry.google,graph.facebook.com,facebook-hardware.com,analytics.whatsapp.com,crashlogs.whatsapp.net,stat.com.telegram,app-measurement.com,samsung-analytics.com,samsungosp.com,samsungcloudplatform.com,logging.samsungdm.com,connectivitycheck.gstatic.com,telemetry.google.com,analytics.google.com,firebase-settings.crashlytics.com,reports.crashlytics.com,api.crashlytics.com,play.googleapis.com,android.clients.google.com,android-context-data.googleapis.com,safebrowsing.googleapis.com,adjust.com,app.adjust.com,app.tr.adjust.com,tracking.intl.miui.com,api.sec.intl.miui.com,api.ad.intl.xiaomi.com,data.mistat.xiaomi.com,sdkconfig.ad.intl.xiaomi.com,api.omc.samsungdm.com,samsung-directory.edge.hiyaapi.com,capi.samsungcloud.com,gos-api.gos-gsp.io,dir-apis.samsungdm.com,api.gras.samsungdm.com,sspapi-prd.samsungrs.com,sdk.pushmessage.samsung.com,us-api.mcsvc.samsung.com,eu-api.mcsvc.samsung.com,ie-odc.samsungapps.com,in.appcenter.ms,query.hicloud.com,configserverdre.platform.hicloud.com`

</details>

<img src="https://user-images.githubusercontent.com/74038190/212284115-f47cd8ff-2ffb-4b04-b5bf-4d1c14c0247f.gif" width="100%" />

## 📬 Контакты и поддержка

Если у вас возникли вопросы, вы нашли неработающий узел или хотите предложить идею:

* 📧 **Email**: [укажите_ваш_email@example.com]
* 💬 **Telegram**: [Наш канал / Чат поддержки](https://t.me/your_channel)

---

## ⚖️ Disclaimer / Отказ от ответственности

1. Проект создается исключительно в ознакомительных, исследовательских и образовательных целях для изучения технологий маршрутизации и оптимизации сетевого трафика.
2. Автор проекта не предоставляет платных услуг, не владеет приватной сетью серверов в рамках данного репозитория и использует данные исключительно из публичных открытых источников.
3. Пользователь несёт самостоятельную ответственность за соблюдение местного законодательства при использовании любых сетевых конфигураций и программного обеспечения.
