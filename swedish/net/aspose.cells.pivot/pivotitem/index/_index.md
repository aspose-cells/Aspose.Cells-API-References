---
title: "PivotItem.Index"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotItem-egenskap. Hämtar indexet för pivot item i cachefältet"
type: docs
url: /sv/net/aspose.cells.pivot/pivotitem/index/
---
## PivotItem.Index property

Hämtar indexet för pivot item i cachefältet.

```csharp
[Obsolete("Use PivotItem.Position property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Index { get; set; }
```

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd istället PivotItem.Position-egenskapen. Denna metod kommer att tas bort 6 månader senare från och med augusti 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyIndexDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;
            
            // Skapa pivottabell
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Hämta radfältet
            PivotField rowField = pivotTable.RowFields[0];
            
            // Åtkomst till pivot items med Index-egenskapen
            foreach (PivotItem item in rowField.PivotItems)
            {
                Console.WriteLine($"Item: {item.Value}, Index: {item.Index}");
                
                // Dölj objektets detalj med Index-egenskapen
                if (item.Value.ToString() == "Apple")
                {
                    rowField.HideItemDetail(item.Index, true);
                }
            }
            
            // Beräkna och uppdatera pivottabell
            pivotTable.CalculateData();
            pivotTable.RefreshData();
            
            // Spara arbetsboken
            workbook.Save("PivotItemPropertyIndexDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


