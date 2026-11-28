---
title: "SlicerCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SlicerCollection özelliği. Slicer'ı indeksine göre alır"
type: docs
url: /tr/net/aspose.cells.slicers/slicercollection/item/
---
## SlicerCollection indexer (1 of 2)

Slicer'ı indeksine göre alır.

```csharp
public Slicer this[int index] { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Fruit");
            sheet.Cells["B1"].PutValue("Quantity");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("Orange");
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["A4"].PutValue("Banana");
            sheet.Cells["B4"].PutValue(15);

            int pivotIndex = sheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            SlicerCollection slicers = sheet.Slicers;
            int slicerIndex = slicers.Add(pivotTable, "H1", "Fruit");

            Slicer slicerByIndex = slicers[0];
            Console.WriteLine("Slicer Name: " + slicerByIndex.Name);
        }
    }
}
```

### Ayrıca Bakınız

* class [Slicer](../../slicer/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## SlicerCollection indexer (2 of 2)

Slicer'ı slicer'ın adıyla alır.

```csharp
public Slicer this[string name] { get; }
```

### Örnekler

```csharp

[C#]

Slicer slicerByName = slicers["fruit"];
```

### Ayrıca Bakınız

* class [Slicer](../../slicer/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


