---
title: "Klasse PivotDiscreteGroupSettings"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Pivot.PivotDiscreteGroupSettings Klasse. Stellt die diskrete Gruppe des Pivot-Feldes dar"
type: docs
url: /de/net/aspose.cells.pivot/pivotdiscretegroupsettings/
---
## PivotDiscreteGroupSettings class

Stellt die diskrete Gruppe des Pivot-Felds dar.

```csharp
public class PivotDiscreteGroupSettings : PivotFieldGroupSettings
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [DiscreteItems](../../aspose.cells.pivot/pivotdiscretegroupsettings/discreteitems/) { get; } | Liefert die diskreten Elemente. |
| [Items](../../aspose.cells.pivot/pivotdiscretegroupsettings/items/) { get; } | (**Obsolete.**) Liefert die diskreten Elemente. |
| override [Type](../../aspose.cells.pivot/pivotdiscretegroupsettings/type/) { get; } | Liefert den Gruppentyp. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotDiscreteGroupSettingsDemo
    {
        public static void PivotDiscreteGroupSettingsExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hinzufügen einiger Beispieldaten
            worksheet.Cells[0, 0].PutValue("Item");
            worksheet.Cells[0, 1].PutValue("Quantity");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(15);
            worksheet.Cells[3, 0].PutValue("A");
            worksheet.Cells[3, 1].PutValue(10);
            worksheet.Cells[4, 0].PutValue("B");
            worksheet.Cells[4, 1].PutValue(15);

            // Fügen Sie der Arbeitsmappe eine PivotTable hinzu
            int pivotIndex = worksheet.PivotTables.Add("=A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Zeilen- und Datenfelder festlegen
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Zugriff auf das Zeilenfeld
            PivotField pivotField = pivotTable.RowFields[0];
            pivotField.GroupBy(new CustomPiovtFieldGroupItem[] { new CustomPiovtFieldGroupItem("TestItemGroup", new int[] { 0, 1}) }, true);

            // Eine Instanz von PivotDiscreteGroupSettings erstellen
            PivotDiscreteGroupSettings groupSettings = pivotField.GroupSettings as PivotDiscreteGroupSettings;

            // Setzt den Gruppentyp auf Diskret (Diese Eigenschaft ist schreibgeschützt)
            // Den aktuellen Gruppentyp anzeigen
            Console.WriteLine("Group Type: " + groupSettings.Type);

            // Speichere die Arbeitsmappe
            workbook.Save("PivotDiscreteGroupSettingsExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* class [PivotFieldGroupSettings](../pivotfieldgroupsettings/)
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


