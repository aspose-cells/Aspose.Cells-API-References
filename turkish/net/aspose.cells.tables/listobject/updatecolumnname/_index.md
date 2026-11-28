---
title: "ListObject.UpdateColumnName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListObject yöntemi. Tablodaki hücrelere tüm liste sütun adlarını günceller"
type: docs
url: /tr/net/aspose.cells.tables/listobject/updatecolumnname/
---
## ListObject.UpdateColumnName method

Tüm liste sütunlarının adını tablo içindeki hücrelere günceller.

```csharp
public void UpdateColumnName()
```

### Açıklamalar

Tablonun başlık satırındaki hücrelerin değeri, ListColumn adının aynı olması gerekir; Cell.PutValue, performans nedeniyle ListColumn adını otomatik olarak değiştirmez.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ListObjectMethodUpdateColumnNameDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Bir tablo/list nesnesi oluştur
            var listObject = ws.ListObjects[ws.ListObjects.Add(3, 3, 6, 6, true)];
            
            // Tabloya bazı veriler ekleyin
            for (int r = 0; r < 3; r++)
            {
                for (int c = 0; c < 3; c++)
                {
                    if (c > 0)
                        ws.Cells[listObject.StartRow + r, listObject.StartColumn + c].PutValue(r + c);
                    else
                        ws.Cells[listObject.StartRow + r, listObject.StartColumn + c].PutValue("");
                }
            }

            // Sütun adlarını güncelleyin (Column1, Column2 vb. gibi varsayılan adlar ayarlanır)
            listObject.UpdateColumnName();

            // Çalışma kitabını kaydedin
            wb.Save("output.xlsx");

            // Sütun adının güncellendiğini doğrulayın
            Console.WriteLine("First column name: " + ws.Cells[listObject.StartRow, listObject.StartColumn].StringValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


