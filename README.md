<div align="center">

  # 🌐 MiGiTi Proxy Subscriptions

  <p align="center">
    <a href="https://github.com/misha12333211-ctrl/proxy-subs/stargazers">
      <img src="https://img.shields.io/github/stars/misha12333211-ctrl/proxy-subs?style=for-the-badge&color=007EC6&logo=github" alt="Stars">
    </a>
    <a href="https://github.com/misha12333211-ctrl/proxy-subs/commits/main">
      <img src="https://img.shields.io/github/last-commit/misha12333211-ctrl/proxy-subs?style=for-the-badge&color=007EC6&logo=git" alt="Last Commit">
    </a>
    <a href="https://github.com/misha12333211-ctrl/proxy-subs">
      <img src="https://komarev.com/ghpvc/?username=misha12333211-ctrl-proxy-subs&style=for-the-badge&color=007EC6&label=VISITORS" alt="Visitors Count">
    </a>
    <img src="https://img.shields.io/badge/Status-Online-brightgreen?style=for-the-badge&logo=statuspage" alt="Status">
  </p>

  <p align="center">
    <b>🚀 Автоматизированный агрегатор публичных конфигураций V2Ray / Xray с проверкой доступности и фильтрацией пинга.</b>
  </p>

  <p align="center">
    🌐 <a href="https://misha12333211-ctrl.github.io/MiGiTi/"><b>Официальный сайт</b></a> •
    💬 <a href="https://t.me/MiGiTi_Bypass_official_channel"><b>Telegram Канал</b></a> •
    📧 <a href="mailto:Fageter@protonmail.com"><b>Связаться по Email</b></a>
  </p>

</div>

---

## 📌 О ПРОЕКТЕ

Проект создан для увлеченных сетевыми технологиями пользователей, оптимизации сетевого трафика и настройки гибкой маршрутизации домашнего интернета.

База конфигураций формируется из открытых источников: данные автоматически и вручную агрегируются, проходят валидацию по доступности и фильтруются по задержке отклика для обеспечения максимальной стабильности соединения.

> [!NOTE]
> **🚀 Проект активно развивается!**  
> Нам очень нужна ваша поддержка и обратная связь! Делитесь фидбеком, отправляйте репорты в Telegram-канал и предлагайте идеи по улучшению. Сейчас сервисы работают как <mark>агрегатор и фильтр публичных узлов</mark>, но при вашей поддержке планируется расширение инфраструктуры и добавление новых высокоскоростных локаций.

---

## 📡 ССЫЛКИ НА ПОДПИСКИ

> [!TIP]
> **Как использовать:** Выделите нужную ссылку, скопируйте её и вставьте в строку добавления подписки в вашем клиенте.

### 1️⃣ Основные подписки

⚪ **01 MIGITI WHITELIST** *(Прямая маршрутизация для локальных сервисов: Яндекс, VK, Госуслуги)*  
`https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/1.txt`

⚡ **02 MIGITI FAST PING** *(Оптимизированные узлы с низкой задержкой)*  
`https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/2.txt`

🌐 **03 MIGITI UNIVERSAL** *(Универсальный набор: VLESS, VMess, Trojan, Shadowsocks)*  
`https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/3.txt`

🥷 **04 MIGITI STEALTH NEXTGEN** *(Конфигурации VLESS REALITY и современные UDP-протоколы)*  
`https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/4.txt`

---

### 2️⃣ Альтернативные зеркала

*Огромное спасибо репозиторию [vpn-configs-for-russia](https://github.com/igareck/vpn-configs-for-russia), благодаря которому появилась идея использования веб-переводчиков в качестве устойчивых зеркал для обхода блокировок сырых ссылок GitHub.*

<details>
<summary><b>📋 Развернуть список альтернативных зеркал (нажмите для просмотра)</b></summary>

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

---

## 🛠️ КАК ОТБИРАЮТСЯ И ЧИСТЯТСЯ СЕРВЕРЫ

Каждый сервер в подписке проходит обязательную многоэтапную обработку:

- [x] 🔎 **Агрегация** — Сбор данных из публичных каналов и Open-Source репозиториев.
- [x] ⚡ **Ping Validation** — Тестирование RTT-задержки и автоматическое отсеивание недоступных узлов.
- [x] 🧹 **Дедупликация** — Очистка дубликатов по ключам шифрования и IP-адресам.
- [x] ⚪ **Валидация SNI** — Проверка корректности работы TLS/SNI заголовков.

---

## ⚙️ НАСТРОЙКИ КЛИЕНТОВ

Для стабильной работы соединений и корректной маршрутизации рекомендуется применить следующие настройки в вашем приложении.

### 🌐 Рекомендуемые DNS-серверы:
*(Выберите один из рабочих вариантов для вашего провайдера)*
* `1.1.1.1` *(Cloudflare)*
* `77.88.8.8` *(Yandex)*
* `dns.alidns.com` *(AliDNS)*
* `https://dns.astracat.ru/DNS-QUERY` *(DoH)*

---

### 📱 Подробная настройка приложений

<details>
<summary>📱 <b>v2rayNG</b> — [<a href="https://github.com/2dust/v2rayNG/releases/tag/2.2.6">Скачать Releases</a>]</summary>

<br>

Перейдите в **Настройки** приложения и выставьте следующие параметры:

1. **Базовые настройки:**
   * **Fake DNS:** 🟢 Включить
   * **MTU:** `1281`
   * **DNS (Удалённый и Внутренний):** Укажите один из рекомендованных DNS из списка выше.
2. **Маршрутизация:**
   * **Режим маршрутизации:** `ipifnonmatch`
   * **Поставщик правил:** `loyalsolider`
   * **Исключения приложений:** Включите и добавьте банковские/локальные приложения в исключения.
3. **Фрагментация (TLS Fragment):**
   * **Длина (Length):** `5-10`
   * **Интервал (Interval):** `5-15`
   * **Максимальное число пакетов:** `20`

</details>

<details>
<summary>📱 <b>Husi</b> — [<a href="https://github.com/xchacha20-poly1305/husi/releases">Скачать Releases</a>]</summary>

<br>

Перейдите в настройки профиля/приложения:

1. **Сетевой стек & DNS:**
   * **Стек (TUN):** `gvisor`
   * **MTU:** `1281`
   * **Fake DNS:** 🟢 Включить *(отметьте опцию «Применять для каждого домена»)*
   * **DNS-сервер:** Один из рекомендованных выше.
2. **Маршрутизация:**
   * **Режим:** `ipifnonmatch`
   * **Поставщик правил:** `loyalsolider`
   * **Исключения приложений:** Настройте раздельное туннелирование для локальных сервисов.
3. **Системные:**
   * **Wakelock:** 🟢 Включить *(предотвращает отключение в фоновом режиме)*

</details>

<details>
<summary>📱 <b>Exclave</b> — [<a href="https://github.com/ExclaveNetwork/Exclave/releases">Скачать Releases</a>]</summary>

<br>

В разделе настроек клиента установите:

1. **Сеть и перехват:**
   * **Стек:** `gvisor`
   * **MTU:** `1281`
   * **DNS:** Введите выбранный DNS-сервер и включите **Маршрутизацию DNS**.
   * **Перехват & Анализ:** Включите *Перехват DNS*, *Анализ трафика* и *Переопределить адрес назначения*.
   * **FakeDNS:** 🟢 Включить.
2. **Маршрутизация и протоколы:**
   * **Маршрутизация:** Поставщик `loyalsolider` \| Режим: `Глобальный`
   * **Параметры протоколов:** 🟢 Включить «Отключить REALITY», 🟢 Включить Hysteria 2.
   * **Фрагментация:** 🟢 Включить фрагментацию TLS \| Метод: *Фрагментация и сегментация*.
3. **Дополнительно:**
   * **Исключения приложений:** Добавьте приложения, требующие прямого подключения.
   * **Wakelock:** 🟢 Включить.

</details>

---

## 💳 ПОДДЕРЖАТЬ ПРОЕКТ (DONATE)

Проект полностью бесплатный, но отбор и поддержка базы требуют времени. Если проект вам пригодился, буду благодарен за поддержку:

* 🟢 **Сбербанк:** [Перевести через Сбер](https://messenger.online.sberbank.ru/sl/HB0CuMt88g020oajp)
* 🧡 **Patreon:** [Мой Patreon](https://www.patreon.com/cw/MiGiTiVlessSubscriptions/shop?sort=published_at)
* 🎁 **DonationAlerts:** [donationalerts.com/r/diagomalacco](https://www.donationalerts.com/r/diagomalacco)
* 💎 **TON Wallet:**  
`UQB4NY_1ula9p2YJpM0kHPEjbJ0mOUK1JNwYUNu9_T2T1Abt`

> [!WARNING]
> **Важное примечание о донатах:**  
> Все финансовые пожертвования (донаты) являются **строго добровольными** и безвозмездными (Donation / Gift). 
> * Автор проекта **не несёт ответственности** за отправленные средства.
> * Пожертвования **не являются оплатой услуг**, не дают никаких коммерческих гарантий, обязательств, персонального обслуживания или подписки на закрытые/платные сервисы.
> * Возврат средств (refund) после отправки не производится. Спасибо за понимание и поддержку!

---

## 📬 КОНТАКТЫ И ПОДДЕРЖКА

Если у вас возникли вопросы, вы нашли неработающий узел или хотите предложить идею:

* 💬 **Telegram:** [MiGiTi Bypass Official Channel](https://t.me/MiGiTi_Bypass_official_channel)
* 📧 **Email:** [Fageter@protonmail.com](mailto:Fageter@protonmail.com)

---

## ⚖️ DISCLAIMER / ОТКАЗ ОТ ОТВЕТСТВЕННОСТИ

1. Проект создается исключительно в ознакомительных, исследовательских и образовательных целях для изучения технологий маршрутизации и оптимизации сетевого трафика.
2. Автор проекта не предоставляет платных услуг, не владеет приватной сетью серверов в рамках данного репозитория и использует данные исключительно из публичных открытых источников.
3. Пользователь несёт самостоятельную ответственность за соблюдение местного законодательства при использовании любых сетевых конфигураций и программного обеспечения.

---
<sub>MiGiTi Proxy Subscriptions • Open Source Project<sub>
