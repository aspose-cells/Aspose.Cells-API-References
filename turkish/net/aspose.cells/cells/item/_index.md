---
title: "Cells.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells özelliği. Belirtilen hücre satır indeksi ve sütun indeksindeki Cell öğesini alır"
type: docs
url: /tr/net/aspose.cells/cells/item/
---
## Cells indexer (1 of 2)

Belirtilen hücre satır indeksi ve sütun indeksindeki [`Cell`](../../cell/) öğesini alır.

```csharp
public Cell this[int row, int column] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| satır | Satır indeksi. |
| sütun | Sütun indeksi. |

### Dönüş Değeri

[`Cell`](../../cell/) nesnesi.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Hücrelere erişmek ve değiştirmek için Item özelliğini kullanma
            cells[0, 0].PutValue("Hello");
            cells[1, 0].PutValue("World");
            
            // Cells aracılığıyla Style özelliğini kullanma
            Style style1 = cells[0, 0].GetStyle();
            style1.Font.IsBold = true;
            cells[0, 0].SetStyle(style1);

            Style style2 = cells[1, 0].GetStyle();
            style2.Font.Color = System.Drawing.Color.Red;
            cells[1, 0].SetStyle(style2);

            // Çalışma kitabını kaydedin
            workbook.Save("CellsPropertyItemDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Cells indexer (2 of 2)

Belirtilen hücre adındaki [`Cell`](../../cell/) öğesini alır.

```csharp
public Cell this[string cellName] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| cellName | Hücre adı, sütun harfi ve satır numarası dahil, örneğin A5. |

### Dönüş Değeri

Bir [`Cell`](../../cell/) nesnesi

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyItemDemo1
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücreler koleksiyonuna eriş
            Cells cells = worksheet.Cells;
            
            // Item özelliğini kullanarak değerleri ayarla
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            
            // Item özelliğini kullanarak bir aralıktaki değerleri ayarla
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(30);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(25);
            
            // Item kullanarak hücre özelliklerine eriş ve değiştir
            Cell cell = cells["B1"];
            Style style = cell.GetStyle();
            style.Font.IsBold = true;
            cell.SetStyle(style);
            
            // Çalışma kitabını kaydedin
            workbook.Save("CellsPropertyItemDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


