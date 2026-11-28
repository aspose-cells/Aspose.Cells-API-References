---
title: "FileFormatInfo.IsProtectedByRMS"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FileFormatInfo özelliği. Dosyanın Microsoft Rights Management Server tarafından korunduğunu gösterir"
type: docs
url: /tr/net/aspose.cells/fileformatinfo/isprotectedbyrms/
---
## FileFormatInfo.IsProtectedByRMS property

Dosyanın Microsoft Rights Management Server tarafından korunduğunu gösterir.

```csharp
public bool IsProtectedByRMS { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatInfoPropertyIsProtectedByRMSDemo
    {
        public static void Run()
        {
            // Örnek 1: RMS korumalı Excel dosyasının korumalı olup olmadığını kontrol edin
            FileFormatInfo info1 = FileFormatUtil.DetectFileFormat("DRMExcel_document.xls");
            Console.WriteLine("Is file protected by RMS: " + info1.IsProtectedByRMS);

            // Örnek 2: Normal Excel dosyasının korumalı olup olmadığını kontrol edin
            FileFormatInfo info2 = FileFormatUtil.DetectFileFormat("upload_simple_1.xls");
            Console.WriteLine("Is file protected by RMS: " + info2.IsProtectedByRMS);
        }
    }
}
```

### Ayrıca Bakınız

* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


