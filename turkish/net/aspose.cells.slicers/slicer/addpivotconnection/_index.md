---
title: "Slicer.AddPivotConnection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Slicer yöntemi. PivotTable bağlantısı ekler"
type: docs
url: /tr/net/aspose.cells.slicers/slicer/addpivotconnection/
---
## Slicer.AddPivotConnection method

PivotTable bağlantısı ekler.

```csharp
public void AddPivotConnection(PivotTable pivot)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivot | PivotTable | PivotTable nesnesi |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerMethodAddPivotConnectionWithPivotTableDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri ekle
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B2"].Value = 10;
            cells["B3"].Value = 15;
            cells["B4"].Value = 5;

            // Özet tablo oluştur
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Slicer ekle - düzeltilmiş parametreler
            int slicerIndex = sheet.Slicers.Add(pivotTable, 0, 0, "Slicer1");
            Slicer slicer = sheet.Slicers[slicerIndex];

            // Slicer'a pivot bağlantısı ekle
            slicer.AddPivotConnection(pivotTable);

            // Çalışma kitabını kaydedin
            workbook.Save("SlicerAddPivotConnectionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


