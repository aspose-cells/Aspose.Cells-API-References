---
title: "ListObjectCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListObjectCollection yöntemi. Bir ListObject'i çalışma sayfasına ekler"
type: docs
url: /tr/net/aspose.cells.tables/listobjectcollection/add/
---
## Add(int, int, int, int, bool) {#add}

Çalışma sayfasına bir ListObject ekler.

```csharp
public int Add(int startRow, int startColumn, int endRow, int endColumn, bool hasHeaders)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | Int32 | Liste aralığının başlangıç satırı. |
| startColumn | Int32 | Liste aralığının başlangıç satırı. |
| endRow | Int32 | Liste aralığının başlangıç satırı. |
| endColumn | Int32 | Liste aralığının başlangıç satırı. |
| hasHeaders | Boolean | Aralığın başlıkları olup olmadığı. |

### Dönüş Değeri

Yeni ListObject'in indeksi

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ListObjectCollectionMethodAddWithInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir aralıkta verileri doldur
            var range = worksheet.Cells.CreateRange("B3:D4");
            range.Value = new object[,]
            {
                {"Col1", "Col2", "Col3"},
                {100, 200, 300}
            };

            // Int32 parametreleriyle Add yöntemi kullanarak ListObject ekle
            int firstRow = range.FirstRow;
            int firstColumn = range.FirstColumn;
            int endRow = firstRow + range.RowCount - 1;
            int endColumn = firstColumn + range.ColumnCount - 1;
            worksheet.ListObjects.Add(firstRow, firstColumn, endRow, endColumn, true);

            // Toplamları etkinleştir ve bir sütun için formül ayarla
            worksheet.ListObjects[0].ShowTotals = true;
            worksheet.Cells["D5"].Formula = "=SUBTOTAL(109,[Col3])";

            // Çalışma kitabını kaydedin
            workbook.Save("ListObjectAddDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, bool) {#add_1}

Çalışma sayfasına bir ListObject ekler.

```csharp
public int Add(string startCell, string endCell, bool hasHeaders)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startCell | String | Liste aralığının başlangıç hücresi. |
| endCell | String | Liste aralığının son hücresi. |
| hasHeaders | Boolean | Aralığın başlıkları olup olmadığı. |

### Dönüş Değeri

Yeni ListObject'in indeksi

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectCollectionMethodAddWithStringStringBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek verileri doldur
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B3"].PutValue(4);

            // Dize aralık referansları kullanarak liste nesnesi ekle
            ListObjectCollection listObjects = worksheet.ListObjects;
            listObjects.Add("A1", "B3", true);
            
            workbook.Save("ListObjectExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


