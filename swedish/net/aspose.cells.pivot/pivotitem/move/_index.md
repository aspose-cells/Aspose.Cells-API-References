---
title: "PivotItem.Move"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotItem-metod. Flyttar elementet upp eller ner"
type: docs
url: /sv/net/aspose.cells.pivot/pivotitem/move/
---
## Move(int, bool) {#move_1}

Flyttar elementet upp eller ner

```csharp
[Obsolete("Use PivotTable.MoveItem(PivotFieldType, string[],bool,int) method  or PivotItem.Move(int) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void Move(int offset, bool isSameParent)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| förskjutning | Int32 | Antalet för flyttning upp eller ner. Flytta elementet upp om detta är mindre än noll; flytta elementet ner om detta är större än noll. |
| isSameParent | Boolean | Anger om flyttoperationen är i samma föräldranod eller inte |

### Anmärkningar

OBS: Den här metoden är nu föråldrad. Använd istället PivotTable.MoveItem(PivotFieldType, string[],bool,int) eller PivotItem.Move(int)-metoden. Denna metod kommer att tas bort 12 månader senare från och med november 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemMethodMoveWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Skapa exempeldata för pivottabell
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["B3"].PutValue(200);
            sheet.Cells["B4"].PutValue(300);

            // Lägg till pivottabell
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Hämta pivotelement och demonstrera Move-metoden
            PivotItemCollection items = pivotTable.RowFields[0].PivotItems;
            
            // Flytta första elementet till position 1 (andra positionen) med underordnade element
            items[0].Move(1, true);
            
            // Spara arbetsboken
            wb.Save("PivotItemMoveDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Move(int) {#move}

Flyttar objektet upp eller ner i pivåtfältet

```csharp
public void Move(int offset)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| förskjutning | Int32 | Antalet för flyttning upp eller ner. Flytta elementet upp om detta är mindre än noll; flytta elementet ner om detta är större än noll. |

### Se även

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


