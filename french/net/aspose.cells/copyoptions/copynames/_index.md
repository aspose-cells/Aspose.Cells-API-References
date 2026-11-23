---
title: "CopyOptions.CopyNames"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CopyOptions. Indique si les noms sont copiés"
type: docs
url: /fr/net/aspose.cells/copyoptions/copynames/
---
## CopyOptions.CopyNames property

Indique si les noms sont copiés.

```csharp
public bool CopyNames { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyCopyNamesDemo
    {
        public static void Run()
        {
            // Créer un classeur source avec des plages nommées
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            
            // Créer une plage nommée dans le classeur source
            sourceSheet.Cells["A1"].PutValue("Test Value");
            int index = sourceWorkbook.Worksheets.Names.Add("SourceName");
            sourceWorkbook.Worksheets.Names[index].RefersTo = "=Sheet1!$A$1";

            // Créer un classeur de destination
            Workbook destWorkbook = new Workbook();
            
            // Copier la feuille de calcul avec CopyNames=true
            destWorkbook.Worksheets[0].Copy(sourceSheet, new CopyOptions { CopyNames = true });

            // Vérifier que la plage nommée a été copiée
            Name copiedName = destWorkbook.Worksheets.Names["SourceName"];
            if (copiedName != null)
            {
                Console.WriteLine("Named range copied successfully: " + copiedName.RefersTo);
            }
            else
            {
                Console.WriteLine("Named range was not copied");
            }
        }
    }
}
```

### Voir aussi

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


