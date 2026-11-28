---
title: "Enum SheetType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.SheetType enum. Çalışma sayfası türünü belirtir"
type: docs
url: /tr/net/aspose.cells/sheettype/
---
## SheetType enumeration

Çalışma sayfası türünü belirtir.

```csharp
public enum SheetType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| VB | `0` | Visual Basic modülü |
| Worksheet | `1` |  |
| Chart | `2` | Grafik |
| BIFF4Macro | `3` | BIFF4 Makro sayfası |
| InternationalMacro | `4` | Uluslararası Makro sayfası |
| Other | `5` |  |
| Dialog | `6` | İletişim çalışma sayfası |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassSheetTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // 0. indekste Worksheet türünde yeni bir çalışma sayfası ekle
            Worksheet newWorksheet = workbook.Worksheets.Insert(0, SheetType.Worksheet);
            
            // Yeni çalışma sayfasının adını ayarla
            newWorksheet.Name = "InsertedSheet";
            
            // Yeni çalışma sayfasındaki hücrelere eriş ve bazı veriler ekle
            newWorksheet.Cells["A1"].PutValue("This is a new worksheet");
            
            // Çalışma kitabını kaydedin
            workbook.Save("SheetTypeDemoOutput.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


