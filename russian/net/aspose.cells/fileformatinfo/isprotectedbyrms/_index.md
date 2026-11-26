---
title: "FileFormatInfo.IsProtectedByRMS"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FileFormatInfo. Указывает, защищён ли файл сервером Microsoft Rights Management"
type: docs
url: /ru/net/aspose.cells/fileformatinfo/isprotectedbyrms/
---
## FileFormatInfo.IsProtectedByRMS property

Указывает, защищён ли файл сервером Microsoft Rights Management.

```csharp
public bool IsProtectedByRMS { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatInfoPropertyIsProtectedByRMSDemo
    {
        public static void Run()
        {
            // Пример 1: Проверить, защищён ли Excel‑файл, защищённый RMS
            FileFormatInfo info1 = FileFormatUtil.DetectFileFormat("DRMExcel_document.xls");
            Console.WriteLine("Is file protected by RMS: " + info1.IsProtectedByRMS);

            // Пример 2: Проверить, защищён ли обычный файл Excel
            FileFormatInfo info2 = FileFormatUtil.DetectFileFormat("upload_simple_1.xls");
            Console.WriteLine("Is file protected by RMS: " + info2.IsProtectedByRMS);
        }
    }
}
```

### См. также

* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


