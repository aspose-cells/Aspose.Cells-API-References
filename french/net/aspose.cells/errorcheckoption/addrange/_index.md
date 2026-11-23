---
title: "ErrorCheckOption.AddRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ErrorCheckOption. Ajoute une plage influencée par ce paramètre"
type: docs
url: /fr/net/aspose.cells/errorcheckoption/addrange/
---
## ErrorCheckOption.AddRange method

Ajoute une plage influencée par ce paramètre.

```csharp
public int AddRange(CellArea ca)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ca | CellArea | la plage à ajouter. |

### Valeur de retour

l'index de la plage ajoutée dans la liste des plages de ce paramètre.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ErrorCheckOptionMethodAddRangeWithCellAreaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            ErrorCheckOptionCollection optsCollection = sheet.ErrorCheckOptions;
            int index = optsCollection.Add();
            ErrorCheckOption opts = optsCollection[index];
            
            opts.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
            
            // Ajouter des plages en utilisant CellArea
            opts.AddRange(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 1, EndColumn = 3 }); // A1:D2
            opts.AddRange(new CellArea { StartRow = 2, StartColumn = 0, EndRow = 2, EndColumn = 3 }); // A3:D3
            
            // Enregistrez le classeur
            workbook.Save("ErrorCheckOptionMethodAddRangeWithCellAreaDemo.xls");
            
            Console.WriteLine("Workbook saved with error check options.");
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../cellarea/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


