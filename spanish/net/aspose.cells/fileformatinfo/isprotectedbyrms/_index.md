---
title: "FileFormatInfo.IsProtectedByRMS"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FileFormatInfo. Indica si el archivo está protegido por Microsoft Rights Management Server"
type: docs
url: /es/net/aspose.cells/fileformatinfo/isprotectedbyrms/
---
## FileFormatInfo.IsProtectedByRMS property

Indica si el archivo está protegido por Microsoft Rights Management Server.

```csharp
public bool IsProtectedByRMS { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatInfoPropertyIsProtectedByRMSDemo
    {
        public static void Run()
        {
            // Ejemplo 1: Verificar si el archivo de Excel protegido por RMS está protegido
            FileFormatInfo info1 = FileFormatUtil.DetectFileFormat("DRMExcel_document.xls");
            Console.WriteLine("Is file protected by RMS: " + info1.IsProtectedByRMS);

            // Ejemplo 2: Verificar si un archivo Excel normal está protegido
            FileFormatInfo info2 = FileFormatUtil.DetectFileFormat("upload_simple_1.xls");
            Console.WriteLine("Is file protected by RMS: " + info2.IsProtectedByRMS);
        }
    }
}
```

### Ver también

* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


