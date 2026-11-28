---
title: "ColumnCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ColumnCollection özelliği. Sütun indeksine göre bir Column nesnesi alır. Belirtilen sütun indeksi için Column nesnesi daha önce yoksa oluşturulur"
type: docs
url: /tr/net/aspose.cells/columncollection/item/
---
## ColumnCollection indexer

Sütun indeksine göre bir [`Column`](../../column/) nesnesi alır. Belirtilen sütun indeksi için Column nesnesi daha önce yoksa oluşturulur.

```csharp
public Column this[int columnIndex] { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Sütun koleksiyonuna erişin
            ColumnCollection columns = worksheet.Cells.Columns;
            
            // Item özelliğini kullanarak sütunların genişliğini ayarlayın
            columns[0].Width = 10;
            columns[1].Width = 15;
            columns[2].Width = 20;
            
            // Sütun genişliklerini gösterin
            Console.WriteLine("Column 0 Width: " + columns[0].Width);
            Console.WriteLine("Column 1 Width: " + columns[1].Width);
            Console.WriteLine("Column 2 Width: " + columns[2].Width);
            
            // Sütun genişliklerinin doğru ayarlandığını doğrulayın
            if (columns[0].Width != 10 || columns[1].Width != 15 || columns[2].Width != 20)
            {
                throw new Exception("Column widths were not set correctly");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Column](../../column/)
* class [ColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


