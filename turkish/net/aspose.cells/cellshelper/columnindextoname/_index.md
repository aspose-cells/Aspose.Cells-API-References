---
title: "CellsHelper.ColumnIndexToName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellsHelper yöntemi. Sütun indeksine göre sütun adını alır"
type: docs
url: /tr/net/aspose.cells/cellshelper/columnindextoname/
---
## CellsHelper.ColumnIndexToName method

Sütun indeksine göre sütun adını alır.

```csharp
public static string ColumnIndexToName(int column)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | Int32 | Sütun indeksi. |

### Dönüş Değeri

Sütun adı.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodColumnIndexToNameWithInt32Demo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Sütun indeksinden ada dönüşümü göstermek için hücrelere değerler ayarla
            worksheet.Cells["A1"].PutValue("Column Index");
            worksheet.Cells["B1"].PutValue("Column Name");

            // 0-4 indeksleri için ColumnIndexToName'i göster
            for (int i = 0; i < 5; i++)
            {
                worksheet.Cells[i + 1, 0].PutValue(i);
                string columnName = CellsHelper.ColumnIndexToName(i);
                worksheet.Cells[i + 1, 1].PutValue(columnName);
            }

            // Çalışma kitabını kaydedin
            workbook.Save("ColumnIndexToNameDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


