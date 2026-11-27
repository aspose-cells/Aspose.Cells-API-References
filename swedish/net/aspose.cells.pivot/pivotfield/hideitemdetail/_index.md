---
title: "PivotField.HideItemDetail"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField-metod. Anger om den specifika PivotItem i ett pivotfält har dold detalj"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/hideitemdetail/
---
## PivotField.HideItemDetail method

Anger om den specifika PivotItem i ett pivotfält har dold detalj.

```csharp
[Obsolete("Use PivotField.PivotItems[int].IsDetailHidden instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void HideItemDetail(int index, bool isHiddenDetail)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | indexet för pivotItem i pivotField. |
| isHiddenDetail | Boolean | om det specifika PivotItem är dolt |

### Anmärkningar

OBS: Den här metoden är nu föråldrad. Använd istället PivotField.PivotItems[int].IsDetailHidden-egenskapen. Denna metod kommer att tas bort 12 månader senare, från och med augusti 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodHideItemDetailWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok från käll‑Excel‑filen
            Workbook workbook = new Workbook("SampleData.xlsx");
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].PutValue("Region");
            worksheet.Cells["A2"].PutValue("North");
            worksheet.Cells["A3"].PutValue("South");
            worksheet.Cells["A4"].PutValue("East");
            worksheet.Cells["A5"].PutValue("West");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);
            worksheet.Cells["B5"].PutValue(4000);

            // Lägg till pivottabell
            int index = worksheet.PivotTables.Add("A1:B5", "H5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Lägg till fält i områden
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Hämta pivotfältet
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Dölj objektets detalj på index 2 (East) med isHidden=false
            pivotField.HideItemDetail(2, false);
            
            // Uppdatera och beräkna pivottabellsdata
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Spara arbetsboken
            workbook.Save("PivotTable_HideItemDetail_Output.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


