---
title: "OoxmlSaveOptions.EnableZip64"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété OoxmlSaveOptions. Utiliser les extensions ZIP64 lors de l'écriture des archives zip si nécessaire"
type: docs
url: /fr/net/aspose.cells/ooxmlsaveoptions/enablezip64/
---
## OoxmlSaveOptions.EnableZip64 property

Utiliser les extensions ZIP64 lors de l'écriture d'archives zip, si nécessaire.

```csharp
public bool EnableZip64 { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsPropertyEnableZip64Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("Sample data for Zip64 demonstration");
            
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.EnableZip64 = true;
            
            workbook.Save("output_with_zip64.xlsx", saveOptions);
        }
    }
}
```

### Voir aussi

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


