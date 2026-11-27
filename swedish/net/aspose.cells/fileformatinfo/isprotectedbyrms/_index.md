---
title: "FileFormatInfo.IsProtectedByRMS"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FileFormatInfo-egenskap. Anger om filen är skyddad av Microsoft Rights Management Server"
type: docs
url: /sv/net/aspose.cells/fileformatinfo/isprotectedbyrms/
---
## FileFormatInfo.IsProtectedByRMS property

Indikerar om filen är skyddad av Microsoft Rights Management Server.

```csharp
public bool IsProtectedByRMS { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatInfoPropertyIsProtectedByRMSDemo
    {
        public static void Run()
        {
            // Exempel 1: Kontrollera om RMS-skyddad Excel-fil är skyddad
            FileFormatInfo info1 = FileFormatUtil.DetectFileFormat("DRMExcel_document.xls");
            Console.WriteLine("Is file protected by RMS: " + info1.IsProtectedByRMS);

            // Exempel 2: Kontrollera om vanlig Excel-fil är skyddad
            FileFormatInfo info2 = FileFormatUtil.DetectFileFormat("upload_simple_1.xls");
            Console.WriteLine("Is file protected by RMS: " + info2.IsProtectedByRMS);
        }
    }
}
```

### Se även

* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


