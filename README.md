<div align="center">

  # 🌐 MiGiTi Proxy Subscriptions 🌐

  <p align="center">
    <a href="[https://github.com/misha12333211-ctrl/proxy-subs/stargazers](https://github.com/misha12333211-ctrl/proxy-subs/stargazers)">
      <img src="[https://img.shields.io/github/stars/misha12333211-ctrl/proxy-subs?style=for-the-badge&color=007EC6&logo=github](https://img.shields.io/github/stars/misha12333211-ctrl/proxy-subs?style=for-the-badge&color=007EC6&logo=github)" alt="Stars">
    </a>
    <a href="[https://github.com/misha12333211-ctrl/proxy-subs/commits/main](https://github.com/misha12333211-ctrl/proxy-subs/commits/main)">
      <img src="[https://img.shields.io/github/last-commit/misha12333211-ctrl/proxy-subs?style=for-the-badge&color=007EC6&logo=git](https://img.shields.io/github/last-commit/misha12333211-ctrl/proxy-subs?style=for-the-badge&color=007EC6&logo=git)" alt="Last Commit">
    </a>
    <a href="[https://github.com/misha12333211-ctrl/proxy-subs](https://github.com/misha12333211-ctrl/proxy-subs)">
      <img src="[https://img.shields.io/badge/Visitors-Counter-007EC6?style=for-the-badge&logo=googleanalytics&logoColor=white](https://img.shields.io/badge/Visitors-Counter-007EC6?style=for-the-badge&logo=googleanalytics&logoColor=white)" alt="Visitors Count">
    </a>
  </p>

  <p align="center">
    <b>🚀 Автоматизированный агрегатор публичных конфигураций V2Ray / Xray с регулярной проверкой доступности, валидацией SNI и фильтрацией пинга.</b>
  </p>

  <p align="center">
    🔗 <a href="[https://misha12333211-ctrl.github.io/MiGiTi/](https://misha12333211-ctrl.github.io/MiGiTi/)"><b>👉 Перейти на официальный сайт проекта 👈</b></a>
  </p>

</div>

---

## 📌 1. О ПРОЕКТЕ

Привет! Проект создан для пользователей, увлеченных сетевыми технологиями, оптимизацией трафика и настройкой гибкой маршрутизации домашнего интернета.

База конфигураций формируется из открытых источников: данные автоматически и вручную агрегируются, проходят проверку доступности и фильтруются по задержке отклика (RTT) для обеспечения максимальной стабильности соединения.

> [!NOTE]
> **🚀 Статус развития:**  
> Сейчас сервис работает как **автоматический агрегатор и фильтр публичных узлов**. В дальнейшем планируется расширение инфраструктуры и добавление новых высокоскоростных локаций при поддержке сообщества.

---

## 🔗 2. ССЫЛКИ НА ПОДПИСКИ

Скопируйте нужную ссылку и вставьте её в ваш VPN-клиент (*v2rayNG, Husi, Exclave, NekoBox и др.*):

### 🚀 2.1. Основные подписки

⚪ **01 MIGITI WHITELIST** *(Прямая маршрутизация для локальных сервисов: Яндекс, VK, Госуслуги)*
```text
https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/1.txt
```

⚡ **02 MIGITI FAST PING** *(Оптимизированные узлы с низкой задержкой)*
```text
https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/2.txt
```

🌐 **03 MIGITI UNIVERSAL** *(Универсальный набор: VLESS, VMess, Trojan, Shadowsocks)*
```text
https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/3.txt
```

🥷 **04 MIGITI STEALTH NEXTGEN** *(Конфигурации VLESS REALITY и современные UDP-протоколы)*
```text
https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/4.txt
```

---

### 🔄 2.2. Альтернативные зеркала

> [!TIP]  
> Если основные ссылки блокируются вашим провайдером, используйте резервные зеркала ниже.

<details>
<summary><b>📋 Нажмите, чтобы развернуть список альтернативных зеркал</b></summary>

<br>

⚪ **01 MIGITI WHITELIST**
```text
https://translate.yandex.ru/translate?url=https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/1.txt&lang=de-de
```

⚡ **02 MIGITI FAST PING**
```text
https://translate.yandex.ru/translate?url=https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/2.txt&lang=de-de
```

🌐 **03 MIGITI UNIVERSAL**
```text
https://translate.yandex.ru/translate?url=https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/3.txt&lang=de-de
```

🥷 **04 MIGITI STEALTH NEXTGEN**
```text
https://translate.yandex.ru/translate?url=https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/4.txt&lang=de-de
```

</details>

---

## 🛠️ 3. КАК ОТБИРАЮТСЯ И ОЧИЩАЮТСЯ СЕРВЕРЫ

Каждый сервер в подписке проходит многоэтапную обработку:

* 🔎 **Агрегация** — Автоматизированный сбор данных из публичных Telegram-каналов и Open-Source репозиториев.
* ⚡ **Ping Validation** — Тестирование RTT-задержки и автоматическое отсеивание недоступных узлов.
* 🧹 **Дедупликация** — Автоматическое удаление дубликатов по ключам и IP-адресам.
* ⚪ **Валидация SNI** — Проверка корректности и целостности TLS/SNI заголовков.

---

## ⚙️ 4. НАСТРОЙКИ КЛИЕНТОВ И МАРШРУТИЗАЦИИ

> [!IMPORTANT]  
> Для правильного распределения трафика рекомендуется настроить исключения в вашем клиенте.

> [!TIP]
> **Раздельное туннелирование (Split Tunneling):**  
> В настройках клиента перейдите в раздел **«Режим VPN для приложений»** (Per-app proxy) и добавьте локальные сервисы (Госуслуги, Банки, Маркетплейсы), чтобы они работали напрямую мимо VPN.

### 🌐 Рекомендуемые DNS-серверы:
* `1.1.1.1`
* `77.88.8.8`
* `dns.alidns.com`
* `[https://dns.astracat.ru/DNS-QUERY](https://dns.astracat.ru/DNS-QUERY)`

---

### 📱 Инструкции по клиентам:

<details>
<summary>📱 <b>v2rayNG</b> — [<a href="[https://github.com/2dust/v2rayNG/releases/tag/2.2.6](https://github.com/2dust/v2rayNG/releases/tag/2.2.6)">Скачать Releases</a>]</summary>

<br>

| Параметр | Значение / Настройка |
| :--- | :--- |
| **Fake DNS** | 🟢 **Включить** |
| **MTU** | `1281` |
| **DNS (Удалённый и Внутренний)** | Укажите один из списка выше |
| **Маршрутизация** | `ipifnonmatch` |
| **Поставщик правил** | `loyalsolider` |
| **Исключения для приложений** | 🟢 Добавить локальные сервисы |

#### ✂️ Фрагментация (Fragment):
* **Длина (Length):** `5-10`
* **Интервал (Interval):** `5-15`
* **Максимальное число пакетов:** `20`

</details>

<details>
<summary>📱 <b>Husi</b> — [<a href="[https://github.com/xchacha20-poly1305/husi/releases](https://github.com/xchacha20-poly1305/husi/releases)">Скачать Releases</a>]</summary>

<br>

| Параметр | Значение / Настройка |
| :--- | :--- |
| **Стек (TUN)** | `gvisor` |
| **MTU** | `1281` |
| **Fake DNS** | 🟢 **Включить** (Применять для каждого домена) |
| **DNS** | Укажите один из списка выше |
| **Маршрутизация** | `ipifnonmatch` |
| **Поставщик правил** | `loyalsolider` |
| **Исключения для приложений** | 🟢 Добавить локальные сервисы |
| **Дополнительно** | 🟢 Включить **Wakelock** |

</details>

<details>
<summary>📱 <b>Exclave</b> — [<a href="[https://github.com/ExclaveNetwork/Exclave/releases](https://github.com/ExclaveNetwork/Exclave/releases)">Скачать Releases</a>]</summary>

<br>

| Параметр | Значение / Настройка |
| :--- | :--- |
| **Стек** | `gvisor` |
| **MTU** | `1281` |
| **DNS** | Укажите один из списка выше + 🟢 *Включить маршрутизацию DNS* |
| **Перехват & Анализ** | 🟢 Перехват DNS <br> 🟢 Анализ трафика <br> 🟢 Переопределить адрес назначения |
| **Маршрутизация** | Поставщик: `loyalsolider` \| Режим: `Глобальный` |
| **Протоколы** | 🟢 Включить «Отключить REALITY» <br> 🟢 Включить Hysteria 2 |
| **Фрагментация** | 🟢 Включить фрагментацию TLS (*Метод: Фрагментация и сегментация*) |
| **Исключения для приложений** | 🟢 Добавить локальные сервисы |
| **Дополнительно** | 🟢 FakeDNS <br> 🟢 Включить **Wakelock** |

</details>

---

## 🛡️ 5. БЛОКИРОВКА РЕКЛАМЫ И ТЕЛЕМЕТРИИ

Чтобы заблокировать рекламу, аналитику и сбор метрик, создайте в вашем VPN-клиенте новое правило со значением **«Блокировать / Block»** и скопируйте список ниже:

<details>
<summary><b>📋 Нажмите, чтобы открыть и скопировать список правил блокировки</b></summary>

<br>

```text
firebaselogging.googleapis.com,play.googleapis.com,google-analytics.com,ssl.google-analytics.com,doubleclick.net,*.doubleclick.net,pubads.g.doubleclick.net,pagead2.googlesyndication.com,googleadservices.com,domain:firebaseio.com,full:firebaselogging.googleapis.com,full:play.googleapis.com,domain:google-analytics.com,domain:doubleclick.net,full:pagead2.googlesyndication.com,full:googleadservices.com,full:s.youtube.com,full:video-stats.l.google.com,domain:crashlytics.com,domain:app-measurement.com,domain:googletagservices.com,domain:googletagmanager.com,domain:s.youtube.com,domain:video-stats.l.google.com,domain:exile.e.youtube.com,domain:google-analytics.com,domain:ssl.google-analytics.com,domain:stats.g.doubleclick.net,regexp:^.*youtube.*\/ptracking$,regexp:^.*youtube.*\/stream_204$,regexp:^.*youtube.*\/gen_204$,domain:sentry.io,domain:samsung-analytics.com,domain:samsungosp.com,geosite:category-ads-all,domain:sentry.io,domain:crashlytics.com,google-analytics.com,firebaseanalytics.amazonaws.com,firebaseio.com,crashlytics.com,telemetry.google,graph.facebook.com,facebook-hardware.com,analytics.whatsapp.com,crashlogs.whatsapp.net,stat.com.telegram,app-measurement.com,samsung-analytics.com,samsungosp.com,samsungcloudplatform.com,logging.samsungdm.com,connectivitycheck.gstatic.com,telemetry.google.com,analytics.google.com,firebase-settings.crashlytics.com,reports.crashlytics.com,api.crashlytics.com,play.googleapis.com,android.clients.google.com,android-context-data.googleapis.com,safebrowsing.googleapis.com,adjust.com,app.adjust.com,app.tr.adjust.com,tracking.intl.miui.com,api.sec.intl.miui.com,api.ad.intl.xiaomi.com,data.mistat.xiaomi.com,sdkconfig.ad.intl.xiaomi.com,api.omc.samsungdm.com,samsung-directory.edge.hiyaapi.com,capi.samsungcloud.com,gos-api.gos-gsp.io,dir-apis.samsungdm.com,api.gras.samsungdm.com,sspapi-prd.samsungrs.com,sdk.pushmessage.samsung.com,us-api.mcsvc.samsung.com,eu-api.mcsvc.samsung.com,ie-odc.samsungapps.com,in.appcenter.ms,query.hicloud.com,configserverdre.platform.hicloud.com
```

</details>

---

## 📬 6. КОНТАКТЫ И ОБРАТНАЯ СВЯЗЬ

Если у вас возникли вопросы, вы нашли неработающий узел или хотите предложить идею по улучшению проекта:

* 💬 **Telegram-канал:** [MiGiTi Bypass Official Channel](https://t.me/MiGiTi_Bypass_official_channel)
* 📧 **E-mail для связи:** `Fageter@protonmail.com`

---

## ⚠️ 7. DISCLAIMER / ПРАВОВАЯ ИНФОРМАЦИЯ И ДОНАТЫ

> [!WARNING]
> **ПРЕДУПРЕЖДЕНИЕ О ДОНАТАХ И МОШЕННИЧЕСТВЕ:**
> * Проект является **полностью бесплатным и некоммерческим**.
> * **Автор НЕ собирает донаты, пожертвования или материальную помощь!**
> * Любые сборы средств, кошельки, карты или ссылки на оплату от имени этого проекта в сторонних источниках являются **ФЕЙКОМ И МОШЕННИЧЕСТВОМ**. Автор не несет ответственности за переведенные сторонним лицам средства.

1. **Цель проекта:** Проект создан исключительно в ознакомительных, исследовательских и образовательных целях для изучения технологий сетевой маршрутизации и оптимизации интернет-соединения.
2. **Источник данных:** Автор проекта не предоставляет платных услуг, не владеет приватной сетью серверов в рамках данного репозитория и использует информацию из открытых публичных источников.
3. **Ответственность:** Пользователь несёт самостоятельную ответственность за соблюдение местного законодательства при использовании любых сетевых конфигураций и стороннего программного обеспечения.
