---
title: "ListObject.TableStyleType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListObject özelliği. Alır ve yerleşik tablo stilini"
type: docs
url: /tr/net/aspose.cells.tables/listobject/tablestyletype/
---
## ListObject.TableStyleType property

Alır ve yerleşik tablo stilini.

```csharp
public TableStyleType TableStyleType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyTableStyleTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelere örnek veri ekle
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Data {i+1}-{j+1}");
                }
            }
            
            // Liste nesneleri koleksiyonunu al
            ListObjectCollection tables = worksheet.ListObjects;
            
            // Bir tablo ekle
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[0];
            
            // Tablo stilini ayarla
            table.TableStyleType = TableStyleType.TableStyleDark2;
            
            // Çalışma kitabını kaydedin
            workbook.Save("TableStyleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [TableStyleType](../../tablestyletype/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


