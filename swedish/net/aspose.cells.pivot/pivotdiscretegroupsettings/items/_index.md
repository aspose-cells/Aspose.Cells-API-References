---
title: "PivotDiscreteGroupSettings.Items"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotDiscreteGroupSettings-egenskap. Hämtar de diskreta objekten."
type: docs
url: /sv/net/aspose.cells.pivot/pivotdiscretegroupsettings/items/
---
## PivotDiscreteGroupSettings.Items property

Hämtar de diskreta objekten.

```csharp
[Obsolete("Use PivotField.GroupBy(DiscreteGroupItem[], bool) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public CustomPiovtFieldGroupItem[] Items { get; }
```

### Anmärkningar

OBS: Denna metod är nu föråldrad. Använd istället PivotField.GroupBy(DiscreteGroupItem[], bool)-metoden. Denna metod kommer att tas bort 12 månader senare från och med juli 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotDiscreteGroupSettingsPropertyItemsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["A5"].PutValue("Apple");
            worksheet.Cells["A6"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["B5"].PutValue(150);
            worksheet.Cells["B6"].PutValue(250);

            // Skapa pivottabell
            int index = worksheet.PivotTables.Add("A1:B6", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            // Hämta pivot-fältet och gruppera det.
            PivotField pivotField = pivotTable.RowFields[0];
            pivotField.GroupBy(new CustomPiovtFieldGroupItem[0], false);

            // Åtkomst till diskreta gruppinställningar.
            PivotDiscreteGroupSettings groupSettings = pivotField.GroupSettings as PivotDiscreteGroupSettings;

            // Visa aktuella objekt.
            Console.WriteLine("Current Items count: " + groupSettings.Items.Length);
            foreach (CustomPiovtFieldGroupItem item in groupSettings.Items)
            {
                Console.WriteLine("Item: " + item.ToString());
            }

            // Spara arbetsboken
            workbook.Save("PivotDiscreteGroupSettingsItemsDemo.xlsx");
        }
    }
}
```

### Se även

* class [CustomPiovtFieldGroupItem](../../custompiovtfieldgroupitem/)
* class [PivotDiscreteGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


