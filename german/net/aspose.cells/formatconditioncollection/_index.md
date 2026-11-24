---
title: "Klasse FormatConditionCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.FormatConditionCollection Klasse. Stellt bedingte Formatierung dar. Die FormatConditions können bis zu drei bedingte Formate enthalten"
type: docs
url: /de/net/aspose.cells/formatconditioncollection/
---
## FormatConditionCollection class

Stellt die bedingte Formatierung dar. Die FormatConditions können bis zu drei bedingte Formate enthalten.

```csharp
public class FormatConditionCollection
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Count](../../aspose.cells/formatconditioncollection/count/) { get; } | Gibt die Anzahl der Bedingungen zurück. |
| [Item](../../aspose.cells/formatconditioncollection/item/) { get; } | Gibt die Formatierungsbedingung nach Index zurück. |
| [RangeCount](../../aspose.cells/formatconditioncollection/rangecount/) { get; } | Gibt die Anzahl der bedingt formatierten Bereiche zurück. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../aspose.cells/formatconditioncollection/add/)(CellArea, FormatConditionType, OperatorType, string, string) | Fügt eine Formatierungsbedingung und den betroffenen Zellbereich zu den FormatConditions hinzu. Die FormatConditions können bis zu drei bedingte Formate enthalten. Verweise auf andere Tabellenblätter sind in den Formeln der bedingten Formatierung nicht zulässig. |
| [AddArea](../../aspose.cells/formatconditioncollection/addarea/)(CellArea) | Fügt einen bedingt formatierten Zellbereich hinzu. |
| [AddCondition](../../aspose.cells/formatconditioncollection/addcondition/#addcondition)(FormatConditionType) | Füge eine Formatbedingung hinzu. |
| [AddCondition](../../aspose.cells/formatconditioncollection/addcondition/#addcondition_1)(FormatConditionType, OperatorType, string, string) | Fügt eine Formatierungsbedingung hinzu. |
| [GetCellArea](../../aspose.cells/formatconditioncollection/getcellarea/)(int) | Gibt den bedingt formatierten Zellbereich nach Index zurück. |
| [RemoveArea](../../aspose.cells/formatconditioncollection/removearea/#removearea_1)(int) | Entfernt den bedingt formatierten Zellbereich nach Index. |
| [RemoveArea](../../aspose.cells/formatconditioncollection/removearea/#removearea)(int, int, int, int) | Entferne die bedingte Formatierung im Bereich. |
| [RemoveCondition](../../aspose.cells/formatconditioncollection/removecondition/)(int) | Entfernt die Formatierungsbedingung nach Index. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionCollectionDemo
    {
        public static void FormatConditionCollectionExample()
        {
            // Erstelle ein neues Workbook
            Workbook workbook = new Workbook();

            // Hole das erste Arbeitsblatt
            Worksheet sheet = workbook.Worksheets[0];

            // Fügt eine leere bedingte Formatierung hinzu
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Setzt den Bereich der bedingten Formatierung
            CellArea ca = new CellArea { StartRow = 0, EndRow = 0, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(ca);
            ca = new CellArea { StartRow = 1, EndRow = 1, StartColumn = 1, EndColumn = 1 };
            fcs.AddArea(ca);

            // Fügt Bedingungen hinzu
            int conditionIndex1 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");

            // Setzt die Hintergrundfarbe
            FormatCondition fc1 = fcs[conditionIndex1];
            fc1.Style.BackgroundColor = System.Drawing.Color.Red;

            // Die Excel-Datei speichern
            workbook.Save("FormatConditionCollectionExample.xlsx");
            workbook.Save("FormatConditionCollectionExample.pdf");
            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


