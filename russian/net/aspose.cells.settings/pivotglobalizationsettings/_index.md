---
title: "Класс PivotGlobalizationSettings"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Settings.PivotGlobalizationSettings класс. Представляет настройки глобализации для сводных таблиц"
type: docs
url: /ru/net/aspose.cells.settings/pivotglobalizationsettings/
---
## PivotGlobalizationSettings class

Представляет параметры глобализации для сводных таблиц.

```csharp
public class PivotGlobalizationSettings
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PivotGlobalizationSettings](pivotglobalizationsettings/)() | Конструктор по умолчанию. |

## Методы

| Имя | Описание |
| --- | --- |
| virtual [GetFormatOfDayGroup](../../aspose.cells.settings/pivotglobalizationsettings/getformatofdaygroup/)() | Получает формат числа группы дней сводной таблицы. Используется только при группировке поля сводной таблицы по дням. Значение по умолчанию — "d-MMM"; |
| virtual [GetNameOfDataField](../../aspose.cells.settings/pivotglobalizationsettings/getnameofdatafield/)(ConsolidationFunction, string) | Получает отображаемое имя поля данных сводной таблицы. Формат по умолчанию — "Sum Of Field". |
| virtual [GetShortTextOf12Months](../../aspose.cells.settings/pivotglobalizationsettings/getshorttextof12months/)() | Получает все коротко отформатированные строки 12 месяцев. |
| virtual [GetTextOf24Hours](../../aspose.cells.settings/pivotglobalizationsettings/gettextof24hours/)() | Получает все локально отформатированные строки 24 часов. Значение по умолчанию: 12 AM, 1 AM, 2 AM, 3 AM, 4 AM, 5 AM, 6 AM, 7 AM, 8 AM, 9 AM, 10 AM, 11 AM, 12 PM, 1 PM, 2 PM, 3 PM, 4 PM, 5 PM, 6 PM, 7 PM, 8 PM, 9 PM, 10 PM, 11 PM. |
| virtual [GetTextOf4Quarters](../../aspose.cells.settings/pivotglobalizationsettings/gettextof4quarters/)() | Получает локальный текст 4 кварталов. |
| virtual [GetTextOf4Quaters](../../aspose.cells.settings/pivotglobalizationsettings/gettextof4quaters/)() | (**Устарело.**) Получает локальный текст 4 кварталов. |
| virtual [GetTextOfAll](../../aspose.cells.settings/pivotglobalizationsettings/gettextofall/)() | Получает текст метки "(All)" в сводной таблице. |
| virtual [GetTextOfAllPeriods](../../aspose.cells.settings/pivotglobalizationsettings/gettextofallperiods/)() | Получает локализованный текст "All Periods". |
| virtual [GetTextOfColumnLabels](../../aspose.cells.settings/pivotglobalizationsettings/gettextofcolumnlabels/)() | Получает текст метки "Column Labels" в сводной таблице. |
| virtual [GetTextOfDataFieldHeader](../../aspose.cells.settings/pivotglobalizationsettings/gettextofdatafieldheader/)() | Получает текст заголовка поля области значений в сводной таблице. |
| virtual [GetTextOfDays](../../aspose.cells.settings/pivotglobalizationsettings/gettextofdays/)() | Получает локальный текст "Days". |
| virtual [GetTextOfEmptyData](../../aspose.cells.settings/pivotglobalizationsettings/gettextofemptydata/)() | Получает текст метки "(blank)" в сводной таблице. |
| virtual [GetTextOfGrandTotal](../../aspose.cells.settings/pivotglobalizationsettings/gettextofgrandtotal/)() | Получает текст метки "Grand Total" в сводной таблице. |
| virtual [GetTextOfHours](../../aspose.cells.settings/pivotglobalizationsettings/gettextofhours/)() | Получает локальный текст "Hours". |
| virtual [GetTextOfMinutes](../../aspose.cells.settings/pivotglobalizationsettings/gettextofminutes/)() | Получает локальный текст "Minutes". |
| virtual [GetTextOfMonths](../../aspose.cells.settings/pivotglobalizationsettings/gettextofmonths/)() | Получает локальный текст "Months". |
| virtual [GetTextOfMultipleItems](../../aspose.cells.settings/pivotglobalizationsettings/gettextofmultipleitems/)() | Получает текст метки "(Multiple Items)" в сводной таблице. |
| virtual [GetTextOfOr](../../aspose.cells.settings/pivotglobalizationsettings/gettextofor/)() | Получает все локально отформатированные строки "or". |
| virtual [GetTextOfProtectedName](../../aspose.cells.settings/pivotglobalizationsettings/gettextofprotectedname/)(string) | Получает текст для указанного защищённого имени. |
| virtual [GetTextOfProtection](../../aspose.cells.settings/pivotglobalizationsettings/gettextofprotection/)() | (**Obsolete.**) Получает имя защиты в сводной таблице. |
| virtual [GetTextOfQuarters](../../aspose.cells.settings/pivotglobalizationsettings/gettextofquarters/)() | Получите локальный текст "Quarters". |
| virtual [GetTextOfRange](../../aspose.cells.settings/pivotglobalizationsettings/gettextofrange/)() | Получает локальный текст "Range" |
| virtual [GetTextOfRowLabels](../../aspose.cells.settings/pivotglobalizationsettings/gettextofrowlabels/)() | Получает текст метки "Row Labels" в сводной таблице. |
| virtual [GetTextOfSeconds](../../aspose.cells.settings/pivotglobalizationsettings/gettextofseconds/)() | Получает локальный текст "Seconds" |
| virtual [GetTextOfSubTotal](../../aspose.cells.settings/pivotglobalizationsettings/gettextofsubtotal/)(PivotFieldSubtotalType) | Получает текст типа [`PivotFieldSubtotalType`](../../aspose.cells.pivot/pivotfieldsubtotaltype/) в сводной таблице. |
| virtual [GetTextOfTotal](../../aspose.cells.settings/pivotglobalizationsettings/gettextoftotal/)() | Получает текст метки "Total" в сводной таблице. Вам необходимо переопределить этот метод, когда сводная таблица содержит два или более полей PivotFields в области данных. |
| virtual [GetTextOfYears](../../aspose.cells.settings/pivotglobalizationsettings/gettextofyears/)() | Получает локальный текст "Years". |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Settings;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotGlobalizationSettingsDemo
    {
        public static void PivotGlobalizationSettingsExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить некоторые данные в лист
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Vegetable");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("Fruit");
            worksheet.Cells["B4"].PutValue(150);
            worksheet.Cells["A5"].PutValue("Vegetable");
            worksheet.Cells["B5"].PutValue(250);

            // Создайте сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Добавьте поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Создайте экземпляр PivotGlobalizationSettings
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

            // Продемонстрировать использование различных методов
            Console.WriteLine("Text of Total: " + globalizationSettings.GetTextOfTotal());
            Console.WriteLine("Text of Grand Total: " + globalizationSettings.GetTextOfGrandTotal());
            Console.WriteLine("Text of Multiple Items: " + globalizationSettings.GetTextOfMultipleItems());
            Console.WriteLine("Text of All: " + globalizationSettings.GetTextOfAll());
            Console.WriteLine("Text of Protection: " + globalizationSettings.GetTextOfProtection());
            Console.WriteLine("Text of Column Labels: " + globalizationSettings.GetTextOfColumnLabels());
            Console.WriteLine("Text of Row Labels: " + globalizationSettings.GetTextOfRowLabels());
            Console.WriteLine("Text of Empty Data: " + globalizationSettings.GetTextOfEmptyData());
            Console.WriteLine("Text of Data Field Header: " + globalizationSettings.GetTextOfDataFieldHeader());
            Console.WriteLine("Text of Years: " + globalizationSettings.GetTextOfYears());
            Console.WriteLine("Text of Quarters: " + globalizationSettings.GetTextOfQuarters());
            Console.WriteLine("Text of Months: " + globalizationSettings.GetTextOfMonths());
            Console.WriteLine("Text of Days: " + globalizationSettings.GetTextOfDays());
            Console.WriteLine("Text of Hours: " + globalizationSettings.GetTextOfHours());
            Console.WriteLine("Text of Minutes: " + globalizationSettings.GetTextOfMinutes());
            Console.WriteLine("Text of Seconds: " + globalizationSettings.GetTextOfSeconds());
            Console.WriteLine("Text of Range: " + globalizationSettings.GetTextOfRange());

            // Пример метода GetTextOfProtectedName
            string protectedName = "ProtectedNameExample";
            Console.WriteLine("Text of Protected Name: " + globalizationSettings.GetTextOfProtectedName(protectedName));

            // Пример метода GetTextOfSubTotal
            PivotFieldSubtotalType subTotalType = PivotFieldSubtotalType.Sum;
            Console.WriteLine("Text of SubTotal (Sum): " + globalizationSettings.GetTextOfSubTotal(subTotalType));

            // Сохраните книгу
            workbook.Save("PivotGlobalizationSettingsExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Settings](../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../)


