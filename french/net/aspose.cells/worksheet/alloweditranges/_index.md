---
title: "Worksheet.AllowEditRanges"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Worksheet property. Obtient la collection des plages d'édition autorisées dans la feuille de calcul"
type: docs
url: /fr/net/aspose.cells/worksheet/alloweditranges/
---
## Worksheet.AllowEditRanges property

Obtient la collection des plages d'édition autorisées dans la feuille de calcul.

```csharp
public ProtectedRangeCollection AllowEditRanges { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyAllowEditRangesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une plage d'édition autorisée
            int index = worksheet.AllowEditRanges.Add("r1", 0, 0, 1, 1);
            ProtectedRange range = worksheet.AllowEditRanges[index];
            range.Password = "password123";

            // Protéger la feuille de calcul
            worksheet.Protect(ProtectionType.All);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");

            // Chargez le classeur enregistré pour vérifier
            Workbook verifyWorkbook = new Workbook("output.xlsx");
            ProtectedRange verifyRange = verifyWorkbook.Worksheets[0].AllowEditRanges[0];
            Console.WriteLine("Is protected with password: " + verifyRange.IsProtectedWithPassword);
        }
    }
}
```

### Voir aussi

* class [ProtectedRangeCollection](../../protectedrangecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


