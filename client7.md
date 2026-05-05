---
layout: default
title: Client7 — зарубежные товары в доставке
---

# Client7 — зарубежные товары в доставке

<div class="page-meta">Pair: <code>Бриф_client7</code> → <code>МП_client7</code></div>

## Summary

| Параметр | Значение |
|---|---|
| Тип задачи | Retail media + 360 digital slice |
| Вход | DOCX-бриф: зарубежные товары в доставке, 360-кампания, TV/OOH/radio/digital/SMM/bloggers, фокус МСК/СПБ, усиление регионов, подробная ЦА. |
| Выход | Excel: МП Digital, гео, cover, Ozon/Avito/VK/Weborama/TG/MTS/Hybrid/Bidease/Everest, интересы, подборки TG/VK. |
| Ключевое правило | Из 360-брифа MVP строит только digital-срез и явно отделяет out-of-scope каналы. |
| Главный риск | Большая часть бюджета/сплита добавлена экспертно; нужны правила гео-распределения. |

## Brief fields

| Поле | Значение | Источник | Действие в системе |
|---|---|---|---|
| Кампания | Зарубежные товары | Brief | Контекст подбора |
| Каналы | 360 + digital/SMM/bloggers | Brief | Digital-срез |
| Гео | Фокус/усиление | Brief | Гео-бюджет |
| ЦА | состоятельные/лояльные сегменты | Brief | Интересы и таргетинги |
| Блогеры | упомянуты | Brief | Подборки TG/VK |

## Media plan structure

| Лист / блок | Назначение |
|---|---|
| МП Digital | Основной digital-план |
| гео | Фокус и усиление |
| cover | Executive summary |
| площадки/data providers | Ozon/Avito/VK/Weborama/TG/etc |
| подборки TG/VK | Influencer/SMM блок |

## Mapping rules

| Из брифа | В медиаплан |
|---|---|
| 360 | только digital scope |
| Фокус/усиление | гео-матрица |
| Retail/delivery | marketplace/programmatic/social |
| ЦА | интересы/таргетинги |

## Planner assumptions

- Programmatic и data providers.
- Cover-summary.
- Бюджетное распределение по городам.

## MVP rules

- 360-бриф → выделять digital scope.
- Retail/delivery → marketplace + social + programmatic.
- Фокусные города → гео-бюджетная матрица.
- Influencer хранить отдельными таблицами.

## Automation checklist

- [ ] Классифицировать тип кампании
- [ ] Выбрать Excel-шаблон
- [ ] Извлечь явные поля из брифа
- [ ] Отделить допущения медиапланера
- [ ] Проверить hard-stop/warning
- [ ] Сформировать Excel-черновик

---

[← Overview](index.html) · [Matrix](matrix.html)
