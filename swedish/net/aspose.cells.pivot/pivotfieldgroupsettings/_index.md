---
title: "Klass PivotFieldGroupSettings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Pivot.PivotFieldGroupSettings-klass. Representerar gruppinställningen för pivotfält"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfieldgroupsettings/
---
## PivotFieldGroupSettings class

Representerar gruppinställningen för pivottfältet.

```csharp
public class PivotFieldGroupSettings
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [PivotFieldGroupSettings](pivotfieldgroupsettings/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| virtual [Type](../../aspose.cells.pivot/pivotfieldgroupsettings/type/) { get; } | Hämtar grupptypen för pivotfält. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldGroupSettingsDemo
    {
        public static void PivotFieldGroupSettingsExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data i kalkylbladet
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[3, 0].Value = "Cherry";
            worksheet.Cells[4, 0].Value = "Date";

            worksheet.Cells[0, 1].Value = "Amount";
            worksheet.Cells[1, 1].Value = 50;
            worksheet.Cells[2, 1].Value = 60;
            worksheet.Cells[3, 1].Value = 70;
            worksheet.Cells[4, 1].Value = 80;

            // Lägg till en pivottabell i kalkylbladet
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till fält i pivottabellen
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Amount

            // Åtkomst till radfältet
            PivotField rowField = pivotTable.RowFields[0];
            rowField.GroupBy(new CustomPiovtFieldGroupItem[] { new CustomPiovtFieldGroupItem("TestItemGroup", new int[] { 0, 1 }) }, true);

            // Åtkomst till gruppinställningarna för radfältet
            PivotFieldGroupSettings groupSettings = rowField.GroupSettings;

            // Visa grupptypen för pivotfältet
            Console.WriteLine("Group Type: " + groupSettings.Type);

            // Spara arbetsboken
            workbook.Save("PivotFieldGroupSettingsExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


