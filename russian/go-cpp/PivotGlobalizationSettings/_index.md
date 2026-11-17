---
title: "Класс PivotGlobalizationSettings"
linktitle: "PivotGlobalizationSettings"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс PivotGlobalizationSettings. Инкапсулирует объект, представляющий pivotglobalizationsettings в Go."
type: docs
weight: 200
url: /ru/go-cpp/pivotglobalizationsettings/
---

## PivotGlobalizationSettings class

Представляет настройки глобализации для сводных таблиц.

```go

type PivotGlobalizationSettings struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewPivotGlobalizationSettings](./newpivotglobalizationsettings/) | Конструктор по умолчанию. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetTextOfTotal](./gettextoftotal/) | Получает текст метки "Total" в PivotTable. Необходимо переопределить этот метод, когда PivotTable содержит два или более PivotFields в области данных. |
| [GetTextOfGrandTotal](./gettextofgrandtotal/) | Получает текст метки "Grand Total" в PivotTable. |
| [GetTextOfMultipleItems](./gettextofmultipleitems/) | Получает текст метки "(Multiple Items)" в PivotTable. |
| [GetTextOfAll](./gettextofall/) | Получает текст метки "(All)" в PivotTable. |
| [GetTextOfProtectedName](./gettextofprotectedname/) | Получает текст для указанного защищённого имени. |
| [GetTextOfColumnLabels](./gettextofcolumnlabels/) | Получает текст метки "Column Labels" в PivotTable. |
| [GetTextOfRowLabels](./gettextofrowlabels/) | Получает текст метки "Row Labels" в PivotTable. |
| [GetTextOfEmptyData](./gettextofemptydata/) | Получает текст метки "(blank)" в PivotTable. |
| [GetTextOfDataFieldHeader](./gettextofdatafieldheader/) | Получает текст заголовка поля области значений в PivotTable. |
| [GetShortTextOf12Months](./getshorttextof12months/) | Получает все коротко отформатированные строки 12 месяцев. |
| [GetTextOf24Hours](./gettextof24hours/) | Получает все локально отформатированные строки 24 часов. Значение по умолчанию: 12 AM, 1 AM, 2 AM, 3 AM, 4 AM, 5 AM, 6 AM, 7 AM, 8 AM, 9 AM, 10 AM, 11 AM, 12 PM, 1 PM, 2 PM, 3 PM, 4 PM, 5 PM, 6 PM, 7 PM, 8 PM, 9 PM, 10 PM, 11 PM. |
| [GetTextOfOr](./gettextofor/) | Получает все локально отформатированные строки "or". |
| [GetFormatOfDayGroup](./getformatofdaygroup/) | Получает числовой формат группы дней сводки. Используется только при группировке поля сводки по дням. Значение по умолчанию: "d-MMM"; |
| [GetTextOf4Quaters](./gettextof4quaters/) | Получает локальный текст 4 кварталов. |
| [GetTextOf4Quarters](./gettextof4quarters/) | Получает локальный текст 4 кварталов. |
| [GetTextOfYears](./gettextofyears/) | Получает локальный текст "Years". |
| [GetTextOfQuarters](./gettextofquarters/) | Получить локальный текст "Quarters". |
| [GetTextOfMonths](./gettextofmonths/) | Получает локальный текст "Months". |
| [GetTextOfDays](./gettextofdays/) | Получает локальный текст "Days". |
| [GetTextOfHours](./gettextofhours/) | Получает локальный текст "Hours". |
| [GetTextOfMinutes](./gettextofminutes/) | Получает локальный текст "Minutes". |
| [GetTextOfSeconds](./gettextofseconds/) | Получает локальный текст "Seconds" |
| [GetTextOfRange](./gettextofrange/) | Получает локальный текст "Range" |
| [GetTextOfAllPeriods](./gettextofallperiods/) | Получает локальный текст "All Periods" |
| [GetTextOfSubTotal](./gettextofsubtotal/) | Получает текст типа PivotFieldSubtotalType в PivotTable. |
| [GetNameOfDataField](./getnameofdatafield/) | Получает отображаемое имя поля данных сводной таблицы. Формат по умолчанию — "Sum Of Field". |
