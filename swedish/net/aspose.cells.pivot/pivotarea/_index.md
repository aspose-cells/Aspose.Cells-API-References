---
title: "Klassen PivotArea"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Pivot.PivotArea-klass. Visar det valda området i pivottabellen"
type: docs
url: /sv/net/aspose.cells.pivot/pivotarea/
---
## PivotArea class

Visar det markerade området i pivottabellen.

```csharp
public class PivotArea
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [PivotArea](pivotarea/)(PivotTable) | Visar det valda området i pivottabellen. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AxisType](../../aspose.cells.pivot/pivotarea/axistype/) { get; set; } | Hämtar och anger regionen för pivottabellen som denna regel gäller för. |
| [Filters](../../aspose.cells.pivot/pivotarea/filters/) { get; } | Hämtar alla filter för detta PivotArea. |
| [IsColumnGrandIncluded](../../aspose.cells.pivot/pivotarea/iscolumngrandincluded/) { get; set; } | Anger om kolumnens totalsumma är inkluderad. |
| [IsOutline](../../aspose.cells.pivot/pivotarea/isoutline/) { get; set; } | Anger om regeln hänvisar till ett område som är i kontursläge. |
| [IsRowGrandIncluded](../../aspose.cells.pivot/pivotarea/isrowgrandincluded/) { get; set; } | Anger om radens totalsumma är inkluderad. |
| [OnlyData](../../aspose.cells.pivot/pivotarea/onlydata/) { get; set; } | Anger om endast datavärdena (i dataområdet i vyn) för ett objektval är markerade och inte inkluderar objektetiketterna. |
| [OnlyLabel](../../aspose.cells.pivot/pivotarea/onlylabel/) { get; set; } | Anger om endast datalabels för ett objektval är markerade. |
| [RuleType](../../aspose.cells.pivot/pivotarea/ruletype/) { get; set; } | Hämtar och anger typen av urvalsregel. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [GetCellAreas](../../aspose.cells.pivot/pivotarea/getcellareas/)() | Hämtar cellområden för detta pivområde. |
| [Select](../../aspose.cells.pivot/pivotarea/select/)(PivotFieldType, int, PivotTableSelectionType) | Välj området med filter. |
| [SelectField](../../aspose.cells.pivot/pivotarea/selectfield/#selectfield)(PivotFieldType, PivotField) | Välj ett fält i regionen som ett område. |
| [SelectField](../../aspose.cells.pivot/pivotarea/selectfield/#selectfield_1)(PivotFieldType, string) | Välj ett fält i regionen som ett område. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotAreaDemo
    {
        public static void PivotAreaExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data i kalkylbladet
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[3, 0].Value = "Cherry";
            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[2, 1].Value = 2021;
            worksheet.Cells[3, 1].Value = 2022;
            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 2].Value = 70;

            // Lägg till en pivottabell i kalkylbladet
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:C4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till fält i pivottabellen
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // Skapa en PivotArea-instans
            PivotArea pivotArea = new PivotArea(pivotTable);

            // Ställ in egenskaper för PivotArea
            pivotArea.OnlyData = true;
            pivotArea.OnlyLabel = false;
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.IsColumnGrandIncluded = true;
            pivotArea.AxisType = PivotFieldType.Row;
            pivotArea.RuleType = PivotAreaType.Normal;
            pivotArea.IsOutline = false;

            // Använd Select-metoden för att välja ett specifikt område
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.DataAndLabel);

            // Spara arbetsboken
            workbook.Save("PivotAreaExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


