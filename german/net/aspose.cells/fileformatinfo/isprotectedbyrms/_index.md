---
title: "FileFormatInfo.IsProtectedByRMS"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FileFormatInfo Eigenschaft. Gibt an, ob die Datei vom Microsoft Rights Management Server geschützt ist"
type: docs
url: /de/net/aspose.cells/fileformatinfo/isprotectedbyrms/
---
## FileFormatInfo.IsProtectedByRMS property

Gibt an, ob die Datei durch den Microsoft Rights Management Server geschützt ist.

```csharp
public bool IsProtectedByRMS { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatInfoPropertyIsProtectedByRMSDemo
    {
        public static void Run()
        {
            // Beispiel 1: Prüfen, ob die RMS-geschützte Excel-Datei geschützt ist
            FileFormatInfo info1 = FileFormatUtil.DetectFileFormat("DRMExcel_document.xls");
            Console.WriteLine("Is file protected by RMS: " + info1.IsProtectedByRMS);

            // Beispiel 2: Prüfen, ob eine reguläre Excel-Datei geschützt ist
            FileFormatInfo info2 = FileFormatUtil.DetectFileFormat("upload_simple_1.xls");
            Console.WriteLine("Is file protected by RMS: " + info2.IsProtectedByRMS);
        }
    }
}
```

### Siehe auch

* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


