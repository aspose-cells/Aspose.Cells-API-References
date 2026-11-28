---
title: "ListObject.Resize"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListObject yöntemi. Liste nesnesinin aralığını yeniden boyutlandır"
type: docs
url: /tr/net/aspose.cells.tables/listobject/resize/
---
## ListObject.Resize method

Liste nesnesinin aralığını yeniden boyutlandır.

```csharp
public void Resize(int startRow, int startColumn, int endRow, int endColumn, bool hasHeaders)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | Int32 | Yeni aralığın başlangıç satır indeksi. |
| startColumn | Int32 | Yeni aralığın başlangıç sütun indeksi. |
| endRow | Int32 | Yeni aralığın bitiş satır indeksi. |
| endColumn | Int32 | Yeni aralığın bitiş sütun indeksi. |
| hasHeaders | Boolean | Bu tablonun başlıkları olup olmadığı. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodResizeWithInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue("Item " + (i + 1));
                worksheet.Cells[i, 1].PutValue(i * 10);
            }

            // Bir liste nesnesi oluştur
            int index = worksheet.ListObjects.Add(0, 0, 5, 1, true);
            ListObject listObj = worksheet.ListObjects[index];
            listObj.TableStyleType = TableStyleType.TableStyleLight2;

            // Liste nesnesini yeniden boyutlandır
            listObj.Resize(0, 0, 9, 1, true);

            // Çalışma kitabını kaydedin
            workbook.Save("ResizedListObject.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


