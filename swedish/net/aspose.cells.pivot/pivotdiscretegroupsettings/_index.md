---
title: "Klass PivotDiscreteGroupSettings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Pivot.PivotDiscreteGroupSettings klass. Representerar den diskreta gruppen för pivottfältet"
type: docs
url: /sv/net/aspose.cells.pivot/pivotdiscretegroupsettings/
---
## PivotDiscreteGroupSettings class

Representerar den diskreta gruppen av pivottfältet

```csharp
public class PivotDiscreteGroupSettings : PivotFieldGroupSettings
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [DiscreteItems](../../aspose.cells.pivot/pivotdiscretegroupsettings/discreteitems/) { get; } | Hämtar de diskreta objekten. |
| [Items](../../aspose.cells.pivot/pivotdiscretegroupsettings/items/) { get; } | (**Obsolete.**) Hämtar de diskreta objekten. |
| override [Type](../../aspose.cells.pivot/pivotdiscretegroupsettings/type/) { get; } | Hämtar grupptypen. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägger till exempeldata
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

            // Lägg till en pivottabell i kalkylbladet
            int pivotIndex = worksheet.PivotTables.Add("=A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Ställ in rad- och datafält
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Åtkomst till radfältet
            PivotField pivotField = pivotTable.RowFields[0];
            pivotField.GroupBy(new CustomPiovtFieldGroupItem[] { new CustomPiovtFieldGroupItem("TestItemGroup", new int[] { 0, 1}) }, true);

            // Skapa en instans av PivotDiscreteGroupSettings
            PivotDiscreteGroupSettings groupSettings = pivotField.GroupSettings as PivotDiscreteGroupSettings;

            // Ställ in grupptypen till Discrete (Denna egenskap är skrivskyddad)
            // Visa den aktuella grupptypen
            Console.WriteLine("Group Type: " + groupSettings.Type);

            // Spara arbetsboken
            workbook.Save("PivotDiscreteGroupSettingsExample.xlsx");

            return;
        }
    }
}
```

### Se även

* class [PivotFieldGroupSettings](../pivotfieldgroupsettings/)
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


