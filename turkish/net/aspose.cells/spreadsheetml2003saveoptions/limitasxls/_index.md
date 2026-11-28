---
title: "SpreadsheetML2003SaveOptions.LimitAsXls"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SpreadsheetML2003SaveOptions özelliği. xls olarak sınırlama, maksimum satır indeksi 65535 ve maksimum sütun indeksi 255'tir"
type: docs
url: /tr/net/aspose.cells/spreadsheetml2003saveoptions/limitasxls/
---
## SpreadsheetML2003SaveOptions.LimitAsXls property

xls sınırı olarak, maksimum satır indeksi 65535 ve maksimum sütun indeksi 255'tir.

```csharp
public bool LimitAsXls { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpreadsheetML2003SaveOptionsPropertyLimitAsXlsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook(FileFormatType.Xlsx);
            
            // Hücrelere erişin ve bir aralık oluşturun
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range range = cells.CreateRange("A1", "C5");
            range.Name = "TestRange";
            
            // LimitAsXls = true ile kaydedin
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions()
            {
                LimitAsXls = true
            };
            
            // XLS sınırlamalarıyla SpreadsheetML olarak kaydedin
            workbook.Save("output.xml", saveOptions);
            
            Console.WriteLine("File saved with LimitAsXls=true");
        }
    }
}
```

### Ayrıca Bakınız

* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


