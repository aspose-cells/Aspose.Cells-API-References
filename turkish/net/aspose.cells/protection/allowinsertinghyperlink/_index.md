---
title: "Protection.AllowInsertingHyperlink"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Protection özelliği. Korunan bir çalışma sayfasında hiperlink eklemenin izin verilip verilmediğini temsil eder."
type: docs
url: /tr/net/aspose.cells/protection/allowinsertinghyperlink/
---
## Protection.AllowInsertingHyperlink property

Korunan bir çalışma sayfasında köprü eklemenin izin verilip verilmediğini temsil eder

```csharp
public bool AllowInsertingHyperlink { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowInsertingHyperlinkDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Protection protection = worksheet.Protection;
            protection.AllowInsertingHyperlink = true;
            protection.Password = "password123";

            // İşlevi göstermek için bir hiperlink ekleyin
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");

            workbook.Save("AllowInsertingHyperlinkDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


