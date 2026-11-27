---
title: "Klassen PivotGlobalizationSettings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Settings.PivotGlobalizationSettings-klass. Representerar globaliseringsinställningarna för pivottabeller"
type: docs
url: /sv/net/aspose.cells.settings/pivotglobalizationsettings/
---
## PivotGlobalizationSettings class

Representerar globaliseringsinställningarna för pivottabeller.

```csharp
public class PivotGlobalizationSettings
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [PivotGlobalizationSettings](pivotglobalizationsettings/)() | Standardkonstruktorn. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| virtual [GetFormatOfDayGroup](../../aspose.cells.settings/pivotglobalizationsettings/getformatofdaygroup/)() | Hämtar talformatet för pivottagsgruppen. Används endast när pivottfältet grupperas efter dagar. Standardvärdet är "d-MMM"; |
| virtual [GetNameOfDataField](../../aspose.cells.settings/pivotglobalizationsettings/getnameofdatafield/)(ConsolidationFunction, string) | Hämtar visningsnamnet för datapivottfältet. Standardformatet är "Sum Of Field". |
| virtual [GetShortTextOf12Months](../../aspose.cells.settings/pivotglobalizationsettings/getshorttextof12months/)() | Hämtar alla kortformaterade strängar för 12 månader. |
| virtual [GetTextOf24Hours](../../aspose.cells.settings/pivotglobalizationsettings/gettextof24hours/)() | Hämtar alla lokalt formaterade strängar för 24 timmar. Standardvärdet är 12 AM, 1 AM, 2 AM, 3 AM, 4 AM, 5 AM, 6 AM, 7 AM, 8 AM, 9 AM, 10 AM, 11 AM, 12 PM, 1 PM, 2 PM, 3 PM, 4 PM, 5 PM, 6 PM, 7 PM, 8 PM, 9 PM, 10 PM, 11 PM. |
| virtual [GetTextOf4Quarters](../../aspose.cells.settings/pivotglobalizationsettings/gettextof4quarters/)() | Hämtar den lokala texten för 4 kvartal. |
| virtual [GetTextOf4Quaters](../../aspose.cells.settings/pivotglobalizationsettings/gettextof4quaters/)() | (**Obsolete.**) Hämtar den lokala texten för 4 kvartal. |
| virtual [GetTextOfAll](../../aspose.cells.settings/pivotglobalizationsettings/gettextofall/)() | Hämtar texten för etiketten "(All)" i pivottabellen. |
| virtual [GetTextOfAllPeriods](../../aspose.cells.settings/pivotglobalizationsettings/gettextofallperiods/)() | Hämtar den lokaliserade texten för "All Periods". |
| virtual [GetTextOfColumnLabels](../../aspose.cells.settings/pivotglobalizationsettings/gettextofcolumnlabels/)() | Hämtar texten för etiketten "Column Labels" i pivottabellen. |
| virtual [GetTextOfDataFieldHeader](../../aspose.cells.settings/pivotglobalizationsettings/gettextofdatafieldheader/)() | Hämtar texten för rubriken på värdeområdesfältet i pivottabellen. |
| virtual [GetTextOfDays](../../aspose.cells.settings/pivotglobalizationsettings/gettextofdays/)() | Hämtar den lokala texten för "Days". |
| virtual [GetTextOfEmptyData](../../aspose.cells.settings/pivotglobalizationsettings/gettextofemptydata/)() | Hämtar texten för etiketten "(blank)" i pivottabellen. |
| virtual [GetTextOfGrandTotal](../../aspose.cells.settings/pivotglobalizationsettings/gettextofgrandtotal/)() | Hämtar texten för etiketten "Grand Total" i pivottabellen. |
| virtual [GetTextOfHours](../../aspose.cells.settings/pivotglobalizationsettings/gettextofhours/)() | Hämtar den lokala texten för "Hours". |
| virtual [GetTextOfMinutes](../../aspose.cells.settings/pivotglobalizationsettings/gettextofminutes/)() | Hämtar den lokala texten för "Minutes". |
| virtual [GetTextOfMonths](../../aspose.cells.settings/pivotglobalizationsettings/gettextofmonths/)() | Hämtar den lokala texten för "Months". |
| virtual [GetTextOfMultipleItems](../../aspose.cells.settings/pivotglobalizationsettings/gettextofmultipleitems/)() | Hämtar texten för etiketten "(Multiple Items)" i PivotTable. |
| virtual [GetTextOfOr](../../aspose.cells.settings/pivotglobalizationsettings/gettextofor/)() | Hämtar alla lokalt formaterade strängar för "or". |
| virtual [GetTextOfProtectedName](../../aspose.cells.settings/pivotglobalizationsettings/gettextofprotectedname/)(string) | Hämtar texten för angivet skyddat namn. |
| virtual [GetTextOfProtection](../../aspose.cells.settings/pivotglobalizationsettings/gettextofprotection/)() | (**Obsolete.**) Hämtar skyddsnamnet i pivottabellen. |
| virtual [GetTextOfQuarters](../../aspose.cells.settings/pivotglobalizationsettings/gettextofquarters/)() | Hämta den lokala texten för "Quarters". |
| virtual [GetTextOfRange](../../aspose.cells.settings/pivotglobalizationsettings/gettextofrange/)() | Hämtar den lokala texten för "Range" |
| virtual [GetTextOfRowLabels](../../aspose.cells.settings/pivotglobalizationsettings/gettextofrowlabels/)() | Hämtar texten för etiketten "Row Labels" i PivotTable. |
| virtual [GetTextOfSeconds](../../aspose.cells.settings/pivotglobalizationsettings/gettextofseconds/)() | Hämtar den lokala texten för "Seconds" |
| virtual [GetTextOfSubTotal](../../aspose.cells.settings/pivotglobalizationsettings/gettextofsubtotal/)(PivotFieldSubtotalType) | Hämtar texten för typen [`PivotFieldSubtotalType`](../../aspose.cells.pivot/pivotfieldsubtotaltype/) i PivotTable. |
| virtual [GetTextOfTotal](../../aspose.cells.settings/pivotglobalizationsettings/gettextoftotal/)() | Hämtar texten för etiketten "Total" i PivotTable. Du måste åsidosätta den här metoden när PivotTable innehåller två eller fler PivotFields i dataområdet. |
| virtual [GetTextOfYears](../../aspose.cells.settings/pivotglobalizationsettings/gettextofyears/)() | Hämtar den lokala texten för "Years". |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data i kalkylbladet
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

            // Skapa en pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till fält i pivottabellen
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Skapa en instans av PivotGlobalizationSettings
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

            // Demonstrera användningen av olika metoder
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

            // Exempel på metoden GetTextOfProtectedName
            string protectedName = "ProtectedNameExample";
            Console.WriteLine("Text of Protected Name: " + globalizationSettings.GetTextOfProtectedName(protectedName));

            // Exempel på metoden GetTextOfSubTotal
            PivotFieldSubtotalType subTotalType = PivotFieldSubtotalType.Sum;
            Console.WriteLine("Text of SubTotal (Sum): " + globalizationSettings.GetTextOfSubTotal(subTotalType));

            // Spara arbetsboken
            workbook.Save("PivotGlobalizationSettingsExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Settings](../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../)


