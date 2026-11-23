---
title: "Worksheet.IsProtected"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Indique si la feuille de calcul est protégée"
type: docs
url: /fr/net/aspose.cells/worksheet/isprotected/
---
## Worksheet.IsProtected property

Indique si la feuille de calcul est protégée.

```csharp
public bool IsProtected { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsProtectedDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Protéger le classeur et la première feuille de calcul
            workbook.Protect(ProtectionType.All, "password");
            workbook.Worksheets[0].Protect(ProtectionType.All, "password", null);

            // Vérifiez si la feuille de calcul est protégée
            bool isProtected = workbook.Worksheets[0].IsProtected;
            Console.WriteLine($"Worksheet is protected: {isProtected}");

            // Enregistrez le classeur
            workbook.Save("protected_worksheet.xlsx");

            // Chargez le classeur enregistré et vérifiez la protection
            Workbook loadedWorkbook = new Workbook("protected_worksheet.xlsx");
            Console.WriteLine($"Loaded worksheet is protected: {loadedWorkbook.Worksheets[0].IsProtected}");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


