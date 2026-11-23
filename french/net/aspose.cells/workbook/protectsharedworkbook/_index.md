---
title: "Workbook.ProtectSharedWorkbook"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Protège un classeur partagé"
type: docs
url: /fr/net/aspose.cells/workbook/protectsharedworkbook/
---
## Workbook.ProtectSharedWorkbook method

Protège un classeur partagé.

```csharp
public void ProtectSharedWorkbook(string password)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| mot de passe | String | Mot de passe pour protéger le classeur. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodProtectSharedWorkbookWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook wb = new Workbook();
            
            // Protégez le classeur partagé avec un mot de passe
            wb.ProtectSharedWorkbook("abcd");
            
            // Enregistrez le classeur protégé
            wb.Save("ProtectedSharedWorkbook.xlsx");
            
            // Chargez le classeur protégé
            Workbook wbProtected = new Workbook("ProtectedSharedWorkbook.xlsx");
            
            // Vérifiez l'état de protection
            Console.WriteLine("Workbook is protected: " + wbProtected.Settings.IsProtected);
            
            // Déprotéger le classeur
            wbProtected.UnprotectSharedWorkbook("abcd");
            
            // Enregistrez le classeur non protégé
            wbProtected.Save("UnprotectedSharedWorkbook.xlsx");
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


