---
title: "Class PivotShowValuesSetting"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Pivot.PivotShowValuesSetting class. Representerar inställningarna för hur värden visas när ShowDataAs-beräkningen används."
type: docs
url: /sv/net/aspose.cells.pivot/pivotshowvaluessetting/
---
## PivotShowValuesSetting class

Representerar inställningarna för att visa värden som när beräkningen ShowDataAs används.

```csharp
public class PivotShowValuesSetting
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [BaseFieldIndex](../../aspose.cells.pivot/pivotshowvaluessetting/basefieldindex/) { get; set; } | Representerar basfältet för en ShowDataAs-beräkning när ShowDataAs-beräkningen används. |
| [BaseFieldName](../../aspose.cells.pivot/pivotshowvaluessetting/basefieldname/) { get; } | Hämtar rubrik för pivottabellens basfält. |
| [BaseItemCaption](../../aspose.cells.pivot/pivotshowvaluessetting/baseitemcaption/) { get; } | Hämtar rubrik för pivottabellens objekt i basfältet. |
| [BaseItemIndex](../../aspose.cells.pivot/pivotshowvaluessetting/baseitemindex/) { get; set; } | Representerar det anpassade indexet för pivottabellens objekt i basfältet när ShowDataAs-beräkningen används. |
| [BaseItemPositionType](../../aspose.cells.pivot/pivotshowvaluessetting/baseitempositiontype/) { get; set; } | (**Obsolete.**) Representerar typen av bas‑pivotobjektet i basfältet när ShowDataAs‑beräkningen används. Eftersom PivotItemPosition.Custom endast är för läsning, om du behöver sätta PivotItemPosition.Custom, vänligen sätt attributet PivotField.BaseItemIndex. |
| [CalculationType](../../aspose.cells.pivot/pivotshowvaluessetting/calculationtype/) { get; set; } | (**Obsolete.**) Representerar hur värden för ett datafält visas i pivottabellrapporten. |
| [ShowValuesAs](../../aspose.cells.pivot/pivotshowvaluessetting/showvaluesas/) { get; set; } | Hämtar och anger hur värden för ett datafält visas i pivottabellrapporten. |

## Fält

| Namn | Beskrivning |
| --- | --- |
| const [NextPivotItem](../../aspose.cells.pivot/pivotshowvaluessetting/nextpivotitem/) | Speciellt basobjektindex: använd det efterföljande pivotobjektet. Giltigt för \"Show Values As\"-beräkningar; gäller i Excel 2010 och senare. |
| const [PreviousPivotItem](../../aspose.cells.pivot/pivotshowvaluessetting/previouspivotitem/) | Speciellt basobjektindex: använd det föregående pivotobjektet. Giltigt för \"Show Values As\"-beräkningar; gäller i Excel 2010 och senare. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotShowValuesSettingDemo
    {
        public static void PivotShowValuesSettingExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data i kalkylbladet
            worksheet.Cells[0, 0].Value = "Product";
            worksheet.Cells[0, 1].Value = "Sales";
            worksheet.Cells[1, 0].Value = "A";
            worksheet.Cells[1, 1].Value = 100;
            worksheet.Cells[2, 0].Value = "B";
            worksheet.Cells[2, 1].Value = 150;
            worksheet.Cells[3, 0].Value = "C";
            worksheet.Cells[3, 1].Value = 200;

            // Lägg till en pivottabell i kalkylbladet
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:B4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till fält i pivottabellen
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales

            // Åtkomst till datafältet
            PivotField dataField = pivotTable.DataFields[0];

            // Åtkomst till egenskapen ShowValuesSetting
            PivotShowValuesSetting showValuesSetting = dataField.ShowValuesSetting;

            // Ställ in egenskaper för PivotShowValuesSetting
            showValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfTotal;
            showValuesSetting.BaseFieldIndex = 0; // Base field index
            showValuesSetting.BaseItemPositionType = PivotItemPositionType.Next;
            showValuesSetting.BaseItemIndex = 1; // Base item index

            // Uppdatera och beräkna pivottabellens data
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Spara arbetsboken
            workbook.Save("PivotShowValuesSettingExample.xlsx");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


