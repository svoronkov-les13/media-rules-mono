---
layout: default
title: Client9 — PPTX multi-campaign: OLV + banners
---

# Client9 — PPTX multi-campaign: OLV + banners

<div class="page-meta">Pair: <code>Бриф_client9</code> → <code>МП_client9</code></div>

## Summary

| Параметр | Значение |
|---|---|
| Тип задачи | PPTX multi-campaign parser |
| Вход | PPTX-бриф с несколькими блоками: имидж 1 июня–6 июля, OLV+баннеры, Smart TV/Mobile/Desktop, Smart TV ≤15%, бюджет 11,789 млн; отдельно Инаут 19 мая–30 июня, бюджет 28,783 млн. Есть CPM/CPC бенчи. |
| Выход | Excel: Свод, МП Инаут, Segmento/Ozon/Яндекс/Bidease/Byyd, video/display, CPM, коэффициенты, свод по периодам. |
| Ключевое правило | PPTX надо сначала разбить на campaign blocks и выбрать нужный блок до генерации плана. |
| Главный риск | Без выбора блока система может построить медиаплан не по той кампании. |

## Brief fields

| Поле | Значение | Источник | Действие в системе |
|---|---|---|---|
| Формат | OLV + banners | Brief | Video/display split |
| Устройства | Smart TV/Mobile/Desktop | Brief | Device constraints |
| Smart TV cap | ≤15% | Brief | Hard constraint |
| Бенчи | CPM/CPC | Brief | Контроль ставок |
| Несколько блоков | Имидж + Инаут | Brief | Нужен выбор кампании |

## Media plan structure

| Лист / блок | Назначение |
|---|---|
| Свод | Агрегация бюджетов |
| МП Инаут | Основной выбранный блок |
| площадки | Segmento/Ozon/Яндекс/Bidease/Byyd |
| факт-лист | Исторический benchmark |

## Mapping rules

| Из брифа | В медиаплан |
|---|---|
| PPTX blocks | campaign segmentation |
| OLV+Banners | Video/Display |
| Smart TV cap | ограничение доли |
| CPM/CPC бенчи | контроль диапазонов |

## Planner assumptions

- Выбор блока Инаут.
- Коэффициенты сезонности/гео/частоты/формата.
- Связь с фактом прошлой кампании.

## MVP rules

- PPTX сначала сегментировать.
- Несколько кампаний → требовать выбор.
- Device cap — hard constraint.
- Бенчи использовать для подсветки отклонений.

## Automation checklist

- [ ] Классифицировать тип кампании
- [ ] Выбрать Excel-шаблон
- [ ] Извлечь явные поля из брифа
- [ ] Отделить допущения медиапланера
- [ ] Проверить hard-stop/warning
- [ ] Сформировать Excel-черновик

---

[← Overview](index.html) · [Matrix](matrix.html)
