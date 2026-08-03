# 🌐 MiGiTi Proxy Subscriptions

<p align="center">
  <a href="https://github.com/misha12333211-ctrl/proxy-subs/stargazers">
    <img src="https://img.shields.io/github/stars/misha12333211-ctrl/proxy-subs?style=flat&label=stars&color=007EC6" alt="Stars">
  </a>
  <a href="https://github.com/misha12333211-ctrl/proxy-subs">
    <img src="https://komarev.com/ghpvc/?username=misha12333211-ctrl-proxy-subs&label=Visitors&color=007EC6&style=flat" alt="Visitors">
  </a>
  <a href="https://github.com/misha12333211-ctrl/proxy-subs/issues">
    <img src="https://img.shields.io/github/issues/misha12333211-ctrl/proxy-subs?style=flat&label=issues&color=007EC6" alt="Issues">
  </a>
  <br>
  <a href="https://github.com/misha12333211-ctrl/proxy-subs/commits/main">
    <img src="https://img.shields.io/github/last-commit/misha12333211-ctrl/proxy-subs?style=flat&label=last%20commit&color=007EC6" alt="Last Commit">
  </a>
  <img src="https://img.shields.io/badge/Open%20Source-%F0%9F%A4%8D-brightgreen" alt="Open Source">
  <br>
  <a href="mailto:Fageter@protonmail.com">
    <img src="https://img.shields.io/badge/Email-Fageter%40protonmail.com-007EC6?style=flat&logo=protonmail&logoColor=white" alt="Email">
  </a>
</p>

Бесплатный коллектор подписок и публичных прокси-серверов V2Ray / Xray с регулярной очисткой, фильтрацией задержки и отбором рабочих конфигов.

🔗 **Официальный сайт проекта**: [misha12333211-ctrl.github.io/MiGiTi](https://misha12333211-ctrl.github.io/MiGiTi/)

---

## 📌 О проекте

Привет! Я уже давно увлечён темой обхода блокировок, настройкой прокси и общим апгрейдом домашнего интернета. Уже больше года я постоянный читатель канала **Киберпортал** — именно их контент и активное сообщество дали мне мощный толчок погрузиться во всё это с головой.

Базу подписок я собираю вручную: сам ищу свежие конфигурации в открытом доступе, прогоняю их через тесты и отбираю только те, которые действительно работают, держат стабильную связь и дают адекватный пинг.

---

## 🛠 Как отбираются и чистятся сервера

Каждый сервер в подписке проходит фильтрацию:

1. **Ручной отбор**: Ищу и проверяю новые конфиги в профильных сообществах и Telegram-каналах.
2. **Фильтр задержки (Ping Validation)**: Нерабочие и медленные узлы отсеиваются. В список `FAST PING` попадают только серверы с задержкой до 90 мс.
3. **Чистка дублей**: Убираю повторяющиеся конфигурации и раскладываю их по категориям (Whitelist, Fast Ping, Universal, Stealth NextGen).

---

## ⚙️ Важно: Правильная настройка клиентов

Подписки и узлы могут быть абсолютно любыми, но ключевую роль играет то, как именно настроен ваш клиент (v2rayN, Sing-Box, NekoBox, Happ, FlClash и др.). 

Я потратил очень много времени на тесты: постоянно менял параметры, сравнивал стабильность, замерял скорость и проверял проходимость узлов при сильных блокировках. В итоге я вывел конфигурацию, с которой прокси работают максимально стабильно и без затыков. 

Настоятельно рекомендую выставить в вашем клиенте следующие значения:

* **Fake DNS**: Обязательно включите параметр `Использовать поддельный DNS` (`Fake DNS` / `FakeIP`).
* **MTU**: Установите значение `1281`.
* **DNS (Удаленный и Внутренний)**: Пропишите `1.1.1.1` или `77.88.8.8`.
* **Фрагментация (Fragment)**: Обязательно активируйте.
  * **Длина (Length)**: `5-10`
  * **Интервал (Interval)**: `5-15`
  * **Максимальное число (Max count / packets)**: `20` (если этот параметр есть в вашем клиенте).

---

## 🔗 Ссылки на подписки

Скопируйте и вставьте нужную ссылку в ваш клиент:

### 1. Стандартные подписки (GitHub)

* **01 MIGITI WHITELIST** (Оптимизировано для работы с российскими сервисами: Яндекс, VK, Госуслуги):
  `https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/1.txt`

* **02 MIGITI FAST PING** (Быстрые серверы с пингом до 90 мс для комфортного сёрфинга и игр):
  `https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/2.txt`

* **03 MIGITI UNIVERSAL** (Сборная подписка с разными протоколами: VLESS, VMess, Trojan, Shadowsocks):
  `https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/3.txt`

* **04 MIGITI STEALTH NEXTGEN** (Конфигурации VLESS REALITY и современные UDP-протоколы):
  `https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/4.txt`

---

### 2. Обновление через Яндекс Переводчик (если GitHub заблокирован)

Если GitHub блокируется вашим провайдером или подписка не обновляется напрямую, используйте проксированные ссылки:

* **01 MIGITI WHITELIST**:
  `https://translate.yandex.ru/translate?url=https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/1.txt&lang=de-de`

* **02 MIGITI FAST PING**:
  `https://translate.yandex.ru/translate?url=https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/2.txt&lang=de-de`

* **03 MIGITI UNIVERSAL**:
  `https://translate.yandex.ru/translate?url=https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/3.txt&lang=de-de`

* **04 MIGITI STEALTH NEXTGEN**:
  `https://translate.yandex.ru/translate?url=https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/4.txt&lang=de-de`

> Спасибо авторам репозитория [vpn-configs-for-russia](https://github.com/igareck/vpn-configs-for-russia) за этот полезный лайфхак!

---

## 💳 Поддержать проект (Donate)

Проект полностью бесплатный, но ручной отбор, постоянный отсев мёртвых серверов и поддержка базы требуют времени. Если мой проект вам пригодился, буду благодарен за поддержку:

* 🟢 **Сбербанк**: [Перевести через Сбер](https://messenger.online.sberbank.ru/sl/HB0CuMt88gO20oajp)
* 🧡 **Patreon**: [Мой Patreon](https://www.patreon.com/cw/MiGiTiVlessSubscriptions/shop?sort=published_at)
* 🎁 **DonationAlerts**: [donationalerts.com/r/diagomalacco](https://www.donationalerts.com/r/diagomalacco)
* 💎 **TON Wallet**: `UQB4NY_1ula9p2YJpM0kHPEjbJOmOUK1JNwYUNu9_T2TlAbt`

---

## 📬 Обратная связь

* **Email**: `Fageter@protonmail.com`
* **GitHub Issues**: Пишите вопросы, замечания и предложения в разделе [Issues](https://github.com/misha12333211-ctrl/proxy-subs/issues) репозитория.
