---
title: "Klasse PivotShowValuesSetting"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Pivot.PivotShowValuesSetting‑Klasse. Stellt die Einstellungen zum Anzeigen von Werten dar, wenn die ShowDataAs‑Berechnung verwendet wird."
type: docs
url: /de/net/aspose.cells.pivot/pivotshowvaluessetting/
---
## PivotShowValuesSetting class

Stellt die Einstellungen zum Anzeigen von Werten dar, wenn die ShowDataAs‑Berechnung verwendet wird.

```csharp
public class PivotShowValuesSetting
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BaseFieldIndex](../../aspose.cells.pivot/pivotshowvaluessetting/basefieldindex/) { get; set; } | Stellt das Basisfeld für eine ShowDataAs‑Berechnung dar, wenn die ShowDataAs‑Berechnung verwendet wird. |
| [BaseFieldName](../../aspose.cells.pivot/pivotshowvaluessetting/basefieldname/) { get; } | Liefert die Beschriftung des Pivot‑Basisfelds. |
| [BaseItemCaption](../../aspose.cells.pivot/pivotshowvaluessetting/baseitemcaption/) { get; } | Liefert die Beschriftung des Pivot‑Elements im Basisfeld. |
| [BaseItemIndex](../../aspose.cells.pivot/pivotshowvaluessetting/baseitemindex/) { get; set; } | Stellt den benutzerdefinierten Index des Pivot‑Elements im Basisfeld dar, wenn die ShowDataAs‑Berechnung verwendet wird. |
| [BaseItemPositionType](../../aspose.cells.pivot/pivotshowvaluessetting/baseitempositiontype/) { get; set; } | (**Obsolete.**) Stellt den Typ des Basis‑Pivot‑Elements im Basisfeld dar, wenn die ShowDataAs‑Berechnung verwendet wird. Da PivotItemPosition.Custom nur lesbar ist, müssen Sie, wenn Sie PivotItemPosition.Custom setzen möchten, das Attribut PivotField.BaseItemIndex festlegen. |
| [CalculationType](../../aspose.cells.pivot/pivotshowvaluessetting/calculationtype/) { get; set; } | (**Obsolete.**) Stellt dar, wie Werte eines Datenfelds im Pivot‑Bericht angezeigt werden. |
| [ShowValuesAs](../../aspose.cells.pivot/pivotshowvaluessetting/showvaluesas/) { get; set; } | Liefert und setzt, wie Werte eines Datenfelds im Pivot‑Bericht angezeigt werden. |

## Felder

| Name | Beschreibung |
| --- | --- |
| const [NextPivotItem](../../aspose.cells.pivot/pivotshowvaluessetting/nextpivotitem/) | Spezialer Basis-Element-Index: Verwenden Sie das nachfolgende Pivot-Element. Gültig für "Show Values As"-Berechnungen; wirksam in Excel 2010 und neuer. |
| const [PreviousPivotItem](../../aspose.cells.pivot/pivotshowvaluessetting/previouspivotitem/) | Spezialer Basis-Element-Index: Verwenden Sie das vorherige Pivot-Element. Gültig für "Show Values As"-Berechnungen; wirksam in Excel 2010 und neuer. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt einige Daten hinzu
            worksheet.Cells[0, 0].Value = "Product";
            worksheet.Cells[0, 1].Value = "Sales";
            worksheet.Cells[1, 0].Value = "A";
            worksheet.Cells[1, 1].Value = 100;
            worksheet.Cells[2, 0].Value = "B";
            worksheet.Cells[2, 1].Value = 150;
            worksheet.Cells[3, 0].Value = "C";
            worksheet.Cells[3, 1].Value = 200;

            // Fügen Sie der Arbeitsmappe eine PivotTable hinzu
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:B4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Füge Felder zur Pivot-Tabelle hinzu
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales

            // Zugriff auf das Datenfeld
            PivotField dataField = pivotTable.DataFields[0];

            // Zugriff auf die ShowValuesSetting-Eigenschaft
            PivotShowValuesSetting showValuesSetting = dataField.ShowValuesSetting;

            // Eigenschaften von PivotShowValuesSetting festlegen
            showValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfTotal;
            showValuesSetting.BaseFieldIndex = 0; // Base field index
            showValuesSetting.BaseItemPositionType = PivotItemPositionType.Next;
            showValuesSetting.BaseItemIndex = 1; // Base item index

            // Aktualisieren und berechnen Sie die Pivot-Tabellendaten
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Speichere die Arbeitsmappe
            workbook.Save("PivotShowValuesSettingExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


