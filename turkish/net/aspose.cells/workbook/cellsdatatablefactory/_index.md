---
title: "Workbook.CellsDataTableFactory"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook özelliği. Özel nesnelerden ICellsDataTable oluşturmak için fabrikayı alır"
type: docs
url: /tr/net/aspose.cells/workbook/cellsdatatablefactory/
---
## Workbook.CellsDataTableFactory property

Özel nesnelerden ICellsDataTable oluşturmak için fabrikayı alır.

```csharp
public CellsDataTableFactory CellsDataTableFactory { get; }
```

### Örnekler

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomData
    {
        public int Id { get; set; }
        public string Name { get; set; }
        public int Age { get; set; }
    }

    public class WorkbookPropertyCellsDataTableFactoryDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            List<CustomData> dataList = new List<CustomData>
            {
                new CustomData { Id = 1, Name = "John Doe", Age = 30 },
                new CustomData { Id = 2, Name = "Jane Smith", Age = 25 },
                new CustomData { Id = 3, Name = "Sam Brown", Age = 35 }
            };

            // Workbook özelliğinden CellsDataTableFactory'yi al
            CellsDataTableFactory factory = workbook.CellsDataTableFactory;

            // Listeden veri tablosu oluştur
            ICellsDataTable dataTable = factory.GetInstance(dataList);

            // Verileri çalışma sayfasına içe aktar
            sheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

            // Çıktıları kaydedin
            workbook.Save("CellsDataTableFactoryDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CellsDataTableFactory](../../cellsdatatablefactory/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


