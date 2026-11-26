---
title: "Slicer.Name"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Slicer. Возвращает или задаёт имя указанного среза"
type: docs
url: /ru/net/aspose.cells.slicers/slicer/name/
---
## Slicer.Name property

Возвращает или задает имя указанного slicer

```csharp
public string Name { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerPropertyNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["A3"].PutValue("Vegetable");
            
            int tableIndex = worksheet.ListObjects.Add("A1", "A3", true);
            ListObject table = worksheet.ListObjects[tableIndex];

            int slicerIndex = worksheet.Slicers.Add(table, 0, "B1");
            Slicer slicer = worksheet.Slicers[slicerIndex];
            slicer.Name = "slicer name";

            workbook.Save("SlicerPropertyNameDemoOutput.xlsx");
        }
    }
}
```

### См. также

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


