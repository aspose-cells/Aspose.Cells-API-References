---
title: "FileFormatInfo.IsProtectedByRMS"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FileFormatInfo. Indica se il file è protetto da Microsoft Rights Management Server"
type: docs
url: /it/net/aspose.cells/fileformatinfo/isprotectedbyrms/
---
## FileFormatInfo.IsProtectedByRMS property

Indica se il file è protetto da Microsoft Rights Management Server.

```csharp
public bool IsProtectedByRMS { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatInfoPropertyIsProtectedByRMSDemo
    {
        public static void Run()
        {
            // Esempio 1: Verifica se il file Excel protetto da RMS è protetto
            FileFormatInfo info1 = FileFormatUtil.DetectFileFormat("DRMExcel_document.xls");
            Console.WriteLine("Is file protected by RMS: " + info1.IsProtectedByRMS);

            // Esempio 2: Verifica se il file Excel normale è protetto
            FileFormatInfo info2 = FileFormatUtil.DetectFileFormat("upload_simple_1.xls");
            Console.WriteLine("Is file protected by RMS: " + info2.IsProtectedByRMS);
        }
    }
}
```

### Vedi anche

* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


