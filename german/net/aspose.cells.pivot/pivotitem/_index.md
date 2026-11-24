---
title: "Klasse PivotItem"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Pivot.PivotItem Klasse. Stellt ein Element in einem PivotField-Bericht dar"
type: docs
url: /de/net/aspose.cells.pivot/pivotitem/
---
## PivotItem class

Stellt ein Element in einem PivotField-Bericht dar.

```csharp
public class PivotItem
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Index](../../aspose.cells.pivot/pivotitem/index/) { get; set; } | (**Obsolete.**) Ermittelt den Index des Pivot‑Elements im Cache‑Feld. |
| [IsCalculatedItem](../../aspose.cells.pivot/pivotitem/iscalculateditem/) { get; } | Gibt an, ob dieses Pivot‑Element ein berechnetes Formelelement ist. |
| [IsDetailHidden](../../aspose.cells.pivot/pivotitem/isdetailhidden/) { get; set; } | Ermittelt und legt fest, ob die Details dieses Pivot‑Elements ausgeblendet sind. |
| [IsFormula](../../aspose.cells.pivot/pivotitem/isformula/) { get; set; } | (**Obsolete.**) Gibt an, ob dieses Pivot‑Element ein berechnetes Formelelement ist. |
| [IsHidden](../../aspose.cells.pivot/pivotitem/ishidden/) { get; set; } | Liest und setzt, ob das Pivot-Element ausgeblendet ist. |
| [IsHideDetail](../../aspose.cells.pivot/pivotitem/ishidedetail/) { get; set; } | (**Obsolete.**) Ermittelt und legt fest, ob das Pivot‑Element Details ausblendet. |
| [IsMissing](../../aspose.cells.pivot/pivotitem/ismissing/) { get; } | Gibt an, ob das Element aus der Datenquelle entfernt wurde. |
| [Name](../../aspose.cells.pivot/pivotitem/name/) { get; set; } | Ermittelt den Namen des Pivot-Elements. |
| [Position](../../aspose.cells.pivot/pivotitem/position/) { get; set; } | Angabe des Index dieses Elements in allen PivotItems des Feldes. |
| [PositionInSameParentNode](../../aspose.cells.pivot/pivotitem/positioninsameparentnode/) { get; set; } | (**Obsolete.**) Angabe des Positionsindex in den PivotItems unter demselben übergeordneten Knoten. |
| [Value](../../aspose.cells.pivot/pivotitem/value/) { get; } | Ermittelt den Wert des Pivot-Elements |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetDateTimeValue](../../aspose.cells.pivot/pivotitem/getdatetimevalue/)() | Ermittelt den Datums‑Uhrzeit‑Wert des Pivot-Elements. Wenn der Wert null ist, wird DateTime.MinValue zurückgegeben. |
| [GetDoubleValue](../../aspose.cells.pivot/pivotitem/getdoublevalue/)() | Ermittelt den Double‑Wert des Pivot-Elements. Wenn der Wert null oder keine Zahl ist, wird 0 zurückgegeben. |
| [GetFormula](../../aspose.cells.pivot/pivotitem/getformula/)() | Ermittelt die Formel dieses berechneten Elements. Funktioniert nur, wenn dieses Element ein berechnetes Element ist. |
| [GetStringValue](../../aspose.cells.pivot/pivotitem/getstringvalue/)() | Ermittelt den Zeichenkettenwert des Pivot-Elements. Wenn der Wert null ist, wird "" zurückgegeben. |
| [Move](../../aspose.cells.pivot/pivotitem/move/#move)(int) | Verschiebt das Element nach oben oder unten im Pivot-Feld |
| [Move](../../aspose.cells.pivot/pivotitem/move/#move_1)(int, bool) | (**Obsolete.**) Verschiebt das Element nach oben oder unten |

## Felder

| Name | Beschreibung |
| --- | --- |
| const [AllPageItemsIndex](../../aspose.cells.pivot/pivotitem/allpageitemsindex/) | Sentinel‑Index für alle Seitenobjekte auswählen (0x7FFD, kein gültiger Index) |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemDemo
    {
        public static void PivotItemExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt einige Daten hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["A3"].PutValue("Vegetable");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);

            // Fügen Sie der Arbeitsmappe eine PivotTable hinzu
            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Füge Felder zur Pivot-Tabelle hinzu
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Zugriff auf die Pivot-Elemente
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = pivotField.PivotItems;

            int pivotItemCount = pivotItems.Count;
            Console.WriteLine("Number of Pivot Items: " + pivotItemCount);
            for(int i = 0; i < pivotItemCount; i++)
            {
                PivotItem pivotItem = pivotItems[i];
                // Gib den Namen des Pivot-Elements aus
                Console.WriteLine("Pivot Item Name: " + pivotItem.Name);

                // Eigenschaften festlegen
                pivotItem.IsHidden = false;
                pivotItem.Position = 1;
                pivotItem.IsHideDetail = false;

                // Gib den Wert des Pivot-Elements aus
                Console.WriteLine("Pivot Item Value: " + pivotItem.Value);

                // Methoden verwenden
                string stringValue = pivotItem.GetStringValue();
                double doubleValue = pivotItem.GetDoubleValue();
                DateTime dateTimeValue = pivotItem.GetDateTimeValue();

                Console.WriteLine("String Value: " + stringValue);
                Console.WriteLine("Double Value: " + doubleValue);
                Console.WriteLine("DateTime Value: " + dateTimeValue);
            }

            // Speichere die Arbeitsmappe
            workbook.Save("PivotItemExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


