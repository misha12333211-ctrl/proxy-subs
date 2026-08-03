# 🌐 MiGiTi Proxy Subscriptions

<p align="center">
  <img src="https://img.shields.io/github/stars/misha12333211-ctrl/proxy-subs?style=for-the-badge&color=white" alt="Stars">
  <img src="https://img.shields.io/github/forks/misha12333211-ctrl/proxy-subs?style=for-the-badge&color=white" alt="Forks">
  <img src="https://img.shields.io/github/license/misha12333211-ctrl/proxy-subs?style=for-the-badge&color=white" alt="License">
</p>

Автоматизированный агрегатор и парсер публичных прокси-узлов V2Ray/Xray с умной фильтрацией, валидацией пинга и защитой от рекламы, телеметрии и трекеров.

🔗 **Официальный сайт проекта**: [misha12333211-ctrl.github.io/proxy-subs](https://misha12333211-ctrl.github.io/proxy-subs/)

---

## 📌 О проекте & Вдохновение

Привет! Я увлекаюсь сетевыми технологиями, архитектурой обхода блокировок и оптимизацией VPN/Proxy уже долгое время. Более года я активно слежу за Telegram-каналом **Киберпортал** — являюсь их фанатом и постоянным читателем. Именно их материалы и комьюнити вдохновили меня на глубокое погружение в тему прокси, правила маршрутизации и кастомные конфигурации.

Благодаря огромному опыту в этой сфере, я создал проект **MiGiTi Proxy**, который решает главную проблему большинства публичных подписок — куча «мертвых» узлов, высокая задержка и мусорный трафик.

---

## 🛠 Архитектура Парсера и Серверов

Проект состоит из двух ключевых частей: автоматического пассивного/активного парсера и веб-интерфейса.

### 1. Парсер и Валидатор узлов
Парсер работает в фоновом режиме по расписанию и выполняет следующий цикл:
* **Сбор данных**: Парсинг открытых источников, Telegram-каналов и публичных реестров прокси (VLESS, VMess, Trojan, Shadowsocks).
* **Дедупликация**: Очистка дубликатов по сочетанию `IP:Port:Protocol:UUID`.
* **Health Check & Ping Validation**: Каждая точка проходит реальный тест соединения (TCP Handshake + HTTP GET замер задержки). Узлы с пингом > 90ms отфильтровываются в отдельный список или удаляются.
* **Генерация подписок**: Результаты группируются по категории и записываются в `1.txt`, `2.txt`, `3.txt`, `4.txt`.

### 2. Фильтрация Трафика и Правила Блокировки
Я прекрасно разбираюсь в правилах маршрутизации (GeoIP, Geosite, AdGuard/uBlock списки) и интеграции блокировок на уровне клиентов (v2rayN, Sing-Box, Happ, Nekobox):
* **Anti-Ad & Anti-Tracker**: Очистка трафика от системной телеметрии (Windows, Android, iOS), трекеров аналитики (Google Analytics, Yandex Metrica) и рекламных сетей.
* **RU SNI Optimization**: Специфические конфигурации для белых списков и обхода региональных ограничений.

---

## 🔗 Готовые Подписки

Вы можете добавить эти ссылки напрямую в ваш VPN-клиент:

| № | Название | Описание | Ссылка на подписку |
|---|---|---|---|
| **01** | **MIGITI WHITELIST** | Оптимизировано под домены и сервисы РФ (Яндекс, VK, ГосУслуги) | [`1.txt`](https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/1.txt) |
| **02** | **MIGITI FAST PING** | Быстрые узлы с пингом менее 90 мс для стриминга и игр | [`2.txt`](https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/2.txt) |
| **03** | **MIGITI UNIVERSAL** | Универсальный набор (VLESS, VMess, Trojan, Shadowsocks) | [`3.txt`](https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/3.txt) |
| **04** | **MIGITI STEALTH NEXTGEN** | VLESS REALITY и современные UDP-протоколы | [`4.txt`](https://raw.githubusercontent.com/misha12333211-ctrl/proxy-subs/refs/heads/main/4.txt) |

---

## 💳 Поддержать проект (Donate)

Проект бесплатный и открытый, однако поддержание парсера, оплата серверов валидации и доменов требуют ресурсов. Если проект вам пригодился, вы можете поддержать автора:

* 🟢 **Сбербанк**: [Перевести через Сбер](https://messenger.online.sberbank.ru/sl/HB0CuMt88gO20oajp)
* 💎 **TON Wallet**: `UQB4NY_1ula9p2YJpM0kHPEjbJOmOUK1JNwYUNu9_T2TlAbt`
* 🎁 **DonationAlerts**: [donationalerts.com/r/diagomalacco](https://www.donationalerts.com/r/diagomalacco)

---

## 📬 Контакты и Обратная связь

* **Email**: `Fageter@proronmail.com`
* **GitHub Issues**: Создавайте Issue в этом репозитории для багрепортов и предложений.
