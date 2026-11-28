---
title: "AutoFilter.SetRange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AutoFilter yöntemi. Belirtilen AutoFilter'ın uygulandığı aralığı ayarlar"
type: docs
url: /tr/net/aspose.cells/autofilter/setrange/
---
## AutoFilter.SetRange method

Belirtilen AutoFilter'ın uygulandığı aralığı ayarlar.

```csharp
public void SetRange(int row, int startColumn, int endColumn)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Satır indeksi. |
| startColumn | Int32 | Başlangıç sütun indeksi. |
| endColumn | Int32 | Son sütun indeksi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodSetRangeWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            sheet.Cells["A1"].PutValue("Header");
            sheet.Cells["A2"].PutValue("Data1");
            sheet.Cells["A3"].PutValue("Data2");
            sheet.Cells["A4"].PutValue("Data3");

            // Otomatik filtre aralığını ayarla (firstRow, firstColumn, totalRows)
            sheet.AutoFilter.SetRange(0, 0, 4);

            // Filtreyi uygula
            sheet.AutoFilter.Custom(0, FilterOperatorType.Equal, "Data2");

            // Filtreyi yenile
            sheet.AutoFilter.Refresh();

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


