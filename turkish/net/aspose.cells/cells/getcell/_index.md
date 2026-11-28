---
title: "Cells.GetCell"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Belirtilen hücre satır indeksi ve sütun indeksindeki Cell öğesini veya null değerini alır"
type: docs
url: /tr/net/aspose.cells/cells/getcell/
---
## Cells.GetCell method

Belirtilen hücre satır indeksi ve sütun indeksindeki [`Cell`](../../cell/) öğesini veya null değerini alır.

```csharp
[Obsolete("Use Cells.CheckCell(int row, int column) instead.")]
public Cell GetCell(int row, int column)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Satır indeksi |
| sütun | Int32 | Sütun indeksi |

### Dönüş Değeri

Bir Cell nesnesi mevcutsa Cell nesnesini döndür. Hücre mevcut değilse null döndür.

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen `CheckCell(int row, int column)` yöntemini kullanın. Bu yöntem Şubat 2024'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetCellWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Satır 1, sütun 2'deki hücreye eriş (0 tabanlı indeks)
            Cell cell = worksheet.Cells.GetCell(1, 2);
            
            // Gösterim için değer ve stil ayarla
            cell.PutValue("Test Value");
            Style style = cell.GetStyle();
            style.Font.IsBold = true;
            cell.SetStyle(style);
            
            // Çalışma kitabını kaydedin
            workbook.Save("GetCellDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


