---
title: "Workbook.UnprotectSharedWorkbook"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Déprotège un classeur partagé"
type: docs
url: /fr/net/aspose.cells/workbook/unprotectsharedworkbook/
---
## Workbook.UnprotectSharedWorkbook method

Supprime la protection d’un classeur partagé.

```csharp
public void UnprotectSharedWorkbook(string password)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| mot de passe | String | Mot de passe pour déprotéger le classeur. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodUnprotectSharedWorkbookWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook wb = new Workbook();
            
            // Protégez le classeur partagé avec un mot de passe
            wb.ProtectSharedWorkbook("abcd");
            
            // Enregistrez le classeur protégé
            wb.Save("ProtectedSharedWorkbook.xlsx");
            
            // Rouvrir le classeur
            wb = new Workbook("ProtectedSharedWorkbook.xlsx");
            
            // Déprotéger le classeur partagé avec un mot de passe
            wb.UnprotectSharedWorkbook("abcd");
            
            // Enregistrez le classeur non protégé
            wb.Save("UnprotectedSharedWorkbook.xlsx");
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


