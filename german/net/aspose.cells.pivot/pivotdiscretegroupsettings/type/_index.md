---
title: "PivotDiscreteGroupSettings.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotDiscreteGroupSettings-Eigenschaft. Gibt den Gruppentyp zurück."
type: docs
url: /de/net/aspose.cells.pivot/pivotdiscretegroupsettings/type/
---
## PivotDiscreteGroupSettings.Type property

Liefert den Gruppentyp.

```csharp
public override PivotFieldGroupType Type { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotDiscreteGroupSettingsPropertyTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten
            worksheet.Cells[0, 0].PutValue("Item");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(20);

            // Pivot-Tabelle erstellen
            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Felder hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Elemente gruppieren
            PivotField pivotField = pivotTable.RowFields[0];
            pivotField.GroupBy(new CustomPiovtFieldGroupItem[] { 
                new CustomPiovtFieldGroupItem("Group1", new int[] { 0, 1 }) 
            }, true);

            // Gruppeneinstellungen abrufen und die Type‑Eigenschaft demonstrieren
            PivotDiscreteGroupSettings groupSettings = pivotField.GroupSettings as PivotDiscreteGroupSettings;
            Console.WriteLine("Group Type: " + groupSettings.Type);

            workbook.Save("PivotDiscreteGroupSettingsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [PivotFieldGroupType](../../pivotfieldgrouptype/)
* class [PivotDiscreteGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


