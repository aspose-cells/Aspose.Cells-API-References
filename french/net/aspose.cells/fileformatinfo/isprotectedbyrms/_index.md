---
title: "FileFormatInfo.IsProtectedByRMS"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FileFormatInfo. Indique si le fichier est protégé par Microsoft Rights Management Server"
type: docs
url: /fr/net/aspose.cells/fileformatinfo/isprotectedbyrms/
---
## FileFormatInfo.IsProtectedByRMS property

Indique si le fichier est protégé par Microsoft Rights Management Server.

```csharp
public bool IsProtectedByRMS { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatInfoPropertyIsProtectedByRMSDemo
    {
        public static void Run()
        {
            // Exemple 1 : Vérifier si le fichier Excel protégé par RMS est protégé
            FileFormatInfo info1 = FileFormatUtil.DetectFileFormat("DRMExcel_document.xls");
            Console.WriteLine("Is file protected by RMS: " + info1.IsProtectedByRMS);

            // Exemple 2 : Vérifier si le fichier Excel ordinaire est protégé
            FileFormatInfo info2 = FileFormatUtil.DetectFileFormat("upload_simple_1.xls");
            Console.WriteLine("Is file protected by RMS: " + info2.IsProtectedByRMS);
        }
    }
}
```

### Voir aussi

* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


