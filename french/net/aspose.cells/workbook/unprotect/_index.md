---
title: "Workbook.Unprotect"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Déprotège un classeur"
type: docs
url: /fr/net/aspose.cells/workbook/unprotect/
---
## Workbook.Unprotect method

Supprime la protection d’un classeur.

```csharp
public void Unprotect(string password)
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
    public class WorkbookMethodUnprotectWithStringDemo
    {
        public static void Run()
        {
            // Créez un classeur avec protection
            Workbook workbook = new Workbook();
            workbook.Protect(ProtectionType.All, "book");

            // Déprotégez le classeur avec le mot de passe correct
            workbook.Unprotect("book");

            // Enregistrez le classeur non protégé
            workbook.Save("unprotected_workbook.xlsx");
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


