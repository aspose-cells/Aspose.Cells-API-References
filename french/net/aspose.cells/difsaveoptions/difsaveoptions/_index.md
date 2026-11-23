---
title: "DifSaveOptions.DifSaveOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur DifSaveOptions. Crée les options pour l'enregistrement d'un fichier DIF"
type: docs
url: /fr/net/aspose.cells/difsaveoptions/difsaveoptions/
---
## DifSaveOptions constructor

Crée les options pour enregistrer le fichier DIF.

```csharp
public DifSaveOptions()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DifSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Data");

            DifSaveOptions saveOptions = new DifSaveOptions()
            {
                ClearData = true,
                CreateDirectory = true,
                RefreshChartCache = true
            };

            workbook.Save("DifSaveOptionsOutput.dif", saveOptions);
        }
    }
}
```

### Voir aussi

* class [DifSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


