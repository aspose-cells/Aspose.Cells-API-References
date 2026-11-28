---
title: "CellsHelper.GetDoubleFromDateTime"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellsHelper yöntemi. Tarih saatini çift (double) değere dönüştürür"
type: docs
url: /tr/net/aspose.cells/cellshelper/getdoublefromdatetime/
---
## CellsHelper.GetDoubleFromDateTime method

Tarih saat değerini double değere dönüştür.

```csharp
public static double GetDoubleFromDateTime(DateTime dateTime, bool date1904)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dateTime | DateTime | Tarih saat. |
| date1904 | Boolean | 1904 tarih sistemi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodGetDoubleFromDateTimeWithDateTimeBooleanDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı örneği oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Geçerli tarih ve saati al
            DateTime now = DateTime.Now;
            
            // DateTime'ı CellsHelper kullanarak double'a dönüştür
            double dateDouble = CellsHelper.GetDoubleFromDateTime(now, false);
            
            // A1 hücresine değeri ayarla
            worksheet.Cells["A1"].PutValue(dateDouble);
            
            // Hücreyi tarih olarak gösterecek şekilde biçimlendir
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Number = 14; // Date format
            worksheet.Cells["A1"].SetStyle(style);
            
            // Çalışma kitabını kaydedin
            workbook.Save("DateTimeConversionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


