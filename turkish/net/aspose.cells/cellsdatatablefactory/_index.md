---
title: "Sınıf CellsDataTableFactory"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.CellsDataTableFactory sınıfı. Kullanıcıların rahatlığı için özel nesnelerden ICellsDataTable oluşturmak için bir yardımcı program"
type: docs
url: /tr/net/aspose.cells/cellsdatatablefactory/
---
## CellsDataTableFactory class

Kullanıcının rahatlığı için özel nesnelerden ICellsDataTable oluşturmak için bir yardımcı program.

```csharp
public class CellsDataTableFactory
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance)(double[]) |  |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_6)(ICollection) | Verilen koleksiyondan ICellsDataTable oluşturur. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_3)(int[]) |  |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_8)(object[]) |  |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_1)(double[], bool) | Verilen çift (double) değer dizisinden ICellsDataTable oluşturur. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_2)(double[], string[]) | Verilen çift (double) değer dizisinden ICellsDataTable oluşturur. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_7)(ICollection, bool) | Verilen koleksiyondan ICellsDataTable oluşturur. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_4)(int[], bool) | Verilen tam sayı (integer) değer dizisinden ICellsDataTable oluşturur. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_5)(int[], string[]) | Verilen tam sayı (integer) değer dizisinden ICellsDataTable oluşturur. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_9)(object[], bool) | Verilen nesne dizisinden ICellsDataTable oluşturur. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_10)(object[], string[]) | Verilen nesne dizisinden ICellsDataTable oluşturur. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_11)(object[][], bool, string[]) | Verilen nesne dizisinden bir ICellsDataTable oluşturur. |

### Örnekler

```csharp
using Aspose.Cells;
using System;
using System.Collections.Generic;

namespace AsposeCellsExamples
{
    public class CellsDataTableFactoryDemo
    {
        public static void RunDemo()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            List<CustomData> dataList = new List<CustomData>
            {
                new CustomData { Id = 1, Name = "John Doe", Age = 30 },
                new CustomData { Id = 2, Name = "Jane Smith", Age = 25 },
                new CustomData { Id = 3, Name = "Sam Brown", Age = 35 }
            };

            // Workbook'tan CellsDataTableFactory örneğini alın
            CellsDataTableFactory factory = workbook.CellsDataTableFactory;

            // Özel veri listesinden ICellsDataTable örneği oluşturun
            ICellsDataTable dataTable = factory.GetInstance(dataList);

            // Veri tablosunu A1 hücresinden başlayarak çalışma sayfasına aktarın
            sheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

            // Çalışma kitabını kaydedin
            workbook.Save("CellsDataTableFactoryDemo.xlsx");
            workbook.Save("CellsDataTableFactoryDemo.pdf");
        }
    }

    // Özel veri sınıfı
    public class CustomData
    {
        public int Id { get; set; }
        public string Name { get; set; }
        public int Age { get; set; }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


