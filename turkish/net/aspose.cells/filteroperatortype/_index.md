---
title: "Enum FilterOperatorType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.FilterOperatorType enum'ı. Özel Filtre operatör tipi"
type: docs
url: /tr/net/aspose.cells/filteroperatortype/
---
## FilterOperatorType enumeration

Özel Filtre operatör türü.

```csharp
public enum FilterOperatorType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| LessOrEqual | `0` | LessOrEqual operatörünü temsil eder. |
| LessThan | `1` | LessThan operatörünü temsil eder. |
| Equal | `2` | Equal operatörünü temsil eder. |
| GreaterThan | `3` | GreaterThan operatörünü temsil eder. |
| NotEqual | `4` | NotEqual operatörünü temsil eder. |
| GreaterOrEqual | `5` | GreaterOrEqual operatörünü temsil eder. |
| None | `6` | Karşılaştırma yoktur. |
| BeginsWith | `7` | Metinle başlar. |
| EndsWith | `8` | Metinle biter. |
| Contains | `9` | Metni içerir. |
| NotContains | `10` | Metni içermez. |
| NotBeginsWith | `11` | Metinle başlamaz. |
| NotEndsWith | `12` | Metinle bitmez. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFilterOperatorTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Names");
            worksheet.Cells["A2"].PutValue("Bob");
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["A4"].PutValue("Bobby");
            worksheet.Cells["A5"].PutValue("Tom");
            
            // Otomatik filtre aralığını ayarla
            worksheet.AutoFilter.Range = "A1:A5";
            
            // İsimleri "Bo" ile başlayanları göstermek için özel filtre uygula
            worksheet.AutoFilter.Custom(0, FilterOperatorType.BeginsWith, "Bo");
            
            // Filtreyi yenile
            worksheet.AutoFilter.Refresh();
            
            // Çalışma kitabını kaydedin
            workbook.Save("FilterOperatorTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


