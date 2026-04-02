# 🛡 CyberFortress — InfoSec Tower Defense (Information Security Architect Simulator)

> Стратегический симулятор архитектора информационной безопасности. Стройте эшелонированную защиту, маршрутизируйте трафик через средства защиты информации (СЗИ), защищайте растущую компанию от 15 волн киберугроз.

![Version](https://img.shields.io/badge/version-1.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Tech](https://img.shields.io/badge/tech-Vanilla%20JS-yellow)
![Size](https://img.shields.io/badge/size-~105KB-lightgrey)

## 🎮 Играть

**Один HTML-файл, zero dependencies.**

*Играть можно на планшете и компьютере (под мобилку не оптимизировано)*
- Откройте ссылку: https://borross.github.io/CyberFortress/
- Скачайте и откройте `index.html` в браузере — и играйте.

```
git clone https://github.com/YOUR_USERNAME/cyberfortress.git
open index.html
```

---

## 📖 Описание

CyberFortress — это обучающая tower-defense игра, в которой вы выступаете в роли **Архитектора информационной безопасности**. Ваша задача — выстроить многоуровневую систему защиты компании, которая растёт от стартапа из 10 сотрудников до корпорации в 17 000+ человек.

Каждое средство защиты (СЗИ) — это реальный класс продуктов ИБ: NGFW, SIEM, DLP, EDR, PAM, ZTNA и другие. Угрозы приходят из разных источников (интернет, email, USB, инсайдеры) и требуют разных стратегий защиты. 

### Для кого эта игра

- 🎓 **Студенты ИБ** — изучение архитектуры безопасности в интерактивном формате
- 🏢 **Менеджеры и CISO** — понимание взаимосвязей между СЗИ и приоритизации инвестиций
- 🛡 **Инженеры ИБ** — проверка интуиции по построению эшелонированной защиты
- 🎮 **Все, кому интересна кибербезопасность** — как стратегическая головоломка

---

## ⚡ Ключевые особенности

### 34 средства защиты информации

Реальные классы СЗИ, разделённые по 8 категориям:

| Категория | СЗИ |
|-----------|-----|
| **🟢 Endpoint** | EPP, EDR, FDE, MDM, Sandbox, Hardening, Patch Management |
| **🔵 Network** | NGFW, DNS Filtering, VPN, NDR, WAF, Email Security, DDoS Protection |
| **🟣 Identity** | MFA, IAM/SSO, PAM, ZTNA, PKI, Password Manager |
| **🟠 Data** | DLP, Backup & Recovery, Data Classification |
| **🔴 Operations** | SIEM, SOAR, IRP, TIP, Deception/Honeypots |
| **🔵 Cloud** | CASB, Container Security (CWPP) |
| **🟡 Assessment** | Vulnerability Scanner, Supply Chain/SBOM |
| **🩷 People** | Security Analyst, Security Awareness Training |

### 15 волн киберугроз

Прогрессия от Script Kiddies до Cyber Armageddon:

| Фаза | Волны | Угрозы |
|------|-------|--------|
| **Onboarding** | W1–3 | Разведка, базовые атаки, malware |
| **Ramp-up** | W4–6 | Insider threats, ransomware, vuln exploits |
| **Mid-game** | W7–9 | APT, supply chain, DDoS + exfiltration |
| **Crisis** | W10–12 | Zero-day, multi-vector, data breach |
| **Endgame** | W13–15 | Nation-state, full spectrum, cyber armageddon |

### Механики

- **🔗 Tandem Boost** — связанные СЗИ усиливают друг друга (+2% за связь)
- **🧑‍💻 Security Analyst** — универсальный усилитель (+15% × Lv/3 к связанным СЗИ)
- **🧪 Sandbox** — усиливает NGFW, Email Security, EPP (+10% × Lv/3)
- **📧 Email min 5%** — email-трафик присутствует во всех волнах (минимум 5%)
- **🕵️ Insider routing** — инсайдерские угрозы обходят сетевые СЗИ, маршрутизируются через identity/operations/people + insider-aware СЗИ
- **🏢 Branch Office** — вторая площадка с 1000+ сотрудников, ~40% угроз идут туда
- **📜 Сертификация** — защита от штрафов регулятора (стоимость = текущие вложения)
- **⚖️ Регулятор** — случайная проверка между W11–14 (30 сек предупреждение, штраф ×1.5 invested)

---

## 💰 Экономика

| Параметр | Значение |
|----------|----------|
| Стартовый бюджет | $2,000 |
| Upkeep | 0.5%/с от инвестиций в СЗИ |
| Upkeep scaling | ×(1 + log₂(emp/5) × 25%) |
| Апгрейд | ×1.5 от текущих инвестиций |
| Продажа | 70% от инвестиций |
| Сертификация | = текущие инвестиции (не увеличивает invested) |
| Штраф регулятора | ×1.5 invested за несертифицированные СЗИ |
| Банкротство | Масштабируется с maturity, ×1.2/волну с W12 |
| Награды W11–15 | ×2.5 от базовых |

### Рост компании

| Волна | Сотрудники | Maturity |
|-------|-----------|----------|
| W1 | 10 | Startup |
| W4 | 80 | Small Business |
| W5 | 160 | Medium Business |
| W7 | 640 → 1280 | Large Business (🏢 Branch opens) |
| W9 | 5120 | Enterprise |
| W11 | 10000 | Enterprise |
| W12+ | +1500/волну | Enterprise |

---

## 🎯 Репутация

Репутация (0–100%) — ваш основной индикатор здоровья. При 0% — Game Over.

- **Блокировка угрозы** — +rep% (= штраф за пропуск / 4)
- **Пропуск угрозы** — -rep% (целые числа, масштабируется по maturity)
- Startup: штраф ×1.2 | Small Business: ×1 | Medium: ×0.7 | Large: ×0.5 | Enterprise: ×0.3

| Тип угрозы | Блок $$ | Пропуск $$ | Пропуск rep |
|------------|---------|------------|-------------|
| Reconnaissance | +$4 | -$16 | -1% |
| Attack | +$11 | -$44 | -2% |
| Incident | +$13 | -$52 | -3% |
| Exfiltration | +$16 | -$64 | -3% |
| Vuln Exploit | +$12 | -$48 | -2% |
| Container Threat | +$10 | -$40 | -2% |
| Forensics | +$6 | -$24 | -1% |
| Threat Hunting | +$8 | -$32 | -2% |
| Misconfiguration | +$8 | -$32 | -2% |

---

## 🖥 Интерфейс

- **Изометрическая карта** — перетаскивание (drag), зум (колёсико/+/-), pan mode (двойной клик)
- **Shopbar** — выбор СЗИ, relevance-индикатор для текущей волны
- **Wave Intel** — разведка следующей волны (типы угроз, EPS, награда)
- **Event Log** — все события с миллисекундными метками `[m:ss.mmm]`
- **Context Menu** — ПКМ на СЗИ: Upgrade, Certify 📜, Move, Info, Sell
- **Reference Guide** — полная документация всех механик
- **Admin Panel** — редактирование параметров в реальном времени (SHA-256 auth)
- **Локализация** — EN / RU

---

## 🔧 Техническое

### Архитектура

Один HTML-файл (~105 KB), zero dependencies:
- **HTML** — минифицированная DOM-структура
- **CSS** — cyberpunk-тема с CSS-переменными
- **JS** — canvas-рендер, изометрическая проекция, event-driven game loop

### Рендер

- Canvas 2D с изометрической проекцией
- Batch-рендеринг угроз по цвету (один `fill()` на группу)
- Адаптивная оптимизация: тени (<30 угроз), иконки (<40), skip рендера (>150: каждая 2-я, >250: каждая 3-я)
- HUD обновляется каждые 1–4 кадра в зависимости от нагрузки
- Частицы: лимит 80, ускоренное затухание при высоком EPS

### Маршрутизация трафика

```
Internet → NGFW → Internet-facing SZI → Link traversal → Catchall → EPP fallback
Email    → NGFW (10%) → Email Security → Link traversal → Catchall → EPP fallback  
USB      → Endpoint SZI → Link traversal → Catchall
Insider  → Identity/Operations/People + Insider-aware SZI → Link traversal → Catchall
```

Insider-aware СЗИ: DLP, CASB, ZTNA, VulnScan, Hardening, CWPP, SBOM

### Формулы

```javascript
// Upkeep (Обслуживание СЗИ) per second 
totalUpkeep = Σ(invested × 0.005) × (1 + log₂(emp/5) × 0.25)

// Upgrade cost (Прокачка СЗИ)
upgradeCost = invested × 1.5

// Sell price (Продажа СЗИ)
sellPrice = invested × 0.70

// Certification cost (does NOT increase invested) (Сертификация СЗИ)
certCost = invested

// Regulator penalty (for uncertified SZI) (Штраф за не сертифицированное СЗИ)
penalty = invested × 1.5

// Analyst boost (Усиление СЗИ за счет Аналитика)
bonus = +15% × (displayLevel / 3)

// Sandbox boost (Усиление СЗИ за счет Песочницы)
bonus = +10% × (displayLevel / 3)

// Link bonus (Усиление СЗИ за счет организации эшелонированности)
bonus = +2% per linked neighbour on same grid

// Rep gain on block (Получаение репутации за отраженную атаку)
repGain = MISS_REP[type] / 4

// Bankruptcy threshold (from W12) (Увеличение шкалы проигрыша по банкротству)
debtLimit = maturity.base × 1.2^(wave - 11)
```

---

## 🕹 Как играть

1. **Введите имя** и нажмите Launch Defense
2. **Выберите СЗИ** в shopbar внизу → **кликните на карту** для размещения
3. **Нажмите ▶ Start Wave** для запуска волны
4. **ПКМ на СЗИ** → Upgrade / Certify / Move / Sell
5. **⏸ Pause** — ставьте на паузу, перемещайте СЗИ, покупайте новые
6. **Следите за Wave Intel** — готовьтесь к следующей волне заранее
7. **Сертифицируйте СЗИ 📜** до W11–14 — иначе регулятор оштрафует


Вызовы между которыми придется балансировать:
- Обслуживание СЗИ в секунду (upkeep/s) - чем больше СЗИ и чем оно прокаченнее, тем дороже upkeep/s, также на этот параметр влияет и количество сотрудников, но оно растет не линейно
- В начале игры денег не много и нужно отражать нарастающиее атаки, тщательно изучайте состав будущей волны в виджете "WAVE INTEL" и какие СЗИ помогут вам больше
- Сертификация решений дешевле на не прокачанном СЗИ, поэтому придется искать время, когда это лучше сделать, проверка регулятора происходит между 11 и 14 волной по ее завершению (будет предупреждение с обратным отсчетом в 30 сек)
- Перед 7 волной откроется новый филиал, который тоже нужно будет защищать, через него будет проходить порядка 40% трафика
- Остальные детали смотрите в игре в Reference Guide

<details> 
<summary>### Советы</summary>
- Тщательно изучите в Reference Guide карточки СЗИ, их эффективность и то, какие узрозы они нейтрализуют
  Используйте паузу, чтобы успеть сделать перестановку, когда что-то пошло не по плану
- NGFW + Email Security — обязательный фундамент
- Security Analyst усиливает 7 связанных СЗИ — ставьте его как можно раньше
- Sandbox + Email Security = мощная защита от фишинга
- Branch Office: дублируйте ключевые СЗИ, ~40% угроз идут туда
- Сертифицируйте самые дорогие СЗИ в первую очередь
- На поздних волнах upkeep scaling агрессивный — продавайте неэффективные СЗИ
</details>
---

## 📊 Скриншоты

<img width="1916" height="894" alt="image" src="https://github.com/user-attachments/assets/eb077618-5d4f-4096-bc2c-d877afd3adf4" />

---

## 📝 Changelog

### v1.0
- 34 СЗИ в 8 категориях
- 15 волн с прогрессивной сложностью
- Dual-zone: Main Office + Branch Office
- Сертификация СЗИ и проверка регулятором
- Insider-aware маршрутизация (DLP, CASB, ZTNA, VulnScan, Hardening, CWPP, SBOM)
- Catchall detection — все подходящие СЗИ участвуют в обнаружении
- Email traffic min 5% all waves
- Batch canvas rendering с адаптивной оптимизацией
- Event log с миллисекундными метками
- Admin panel с SHA-256 аутентификацией
- Локализация EN/RU
- Copy Stats — экспорт статистики по завершении

---

## 📄 Лицензия

MIT License — свободное использование, модификация и распространение.

---

<p align="center">
  <b>CyberFortress</b> — learn cybersecurity architecture by playing<br>
  <i>Build. Defend. Survive.</i>
</p>
