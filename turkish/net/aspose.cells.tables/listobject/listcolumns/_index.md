---
title: "ListObject.ListColumns"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListObject özelliği. Bu tablonun ListColumn listesini alır"
type: docs
url: /tr/net/aspose.cells.tables/listobject/listcolumns/
---
## ListObject.ListColumns property

Bu tablonun [`ListColumn`](../../listcolumn/) listesini alır.

```csharp
public ListColumnCollection ListColumns { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyListColumnsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue((i + 1) * (j + 1));
                }
            }

            // Bir liste nesnesi oluştur
            ListObjectCollection listObjects = worksheet.ListObjects;
            int index = listObjects.Add(0, 0, 9, 4, true);
            ListObject listObject = listObjects[index];
            
            // Toplamları etkinleştir ve 5. sütun için hesaplamayı ayarla
            listObject.ShowTotals = true;
            listObject.ListColumns[4].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;
            
            // Tablo stilini uygula
            listObject.TableStyleType = Aspose.Cells.Tables.TableStyleType.TableStyleLight4;

            // Çalışma kitabını kaydedin
            workbook.Save("ListColumnsDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ListColumnCollection](../../listcolumncollection/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


