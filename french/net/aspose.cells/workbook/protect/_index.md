---
title: "Workbook.Protect"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Protège un classeur"
type: docs
url: /fr/net/aspose.cells/workbook/protect/
---
## Workbook.Protect method

Protège un classeur.

```csharp
public void Protect(ProtectionType protectionType, string password)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| protectionType | ProtectionType | Type de protection. |
| mot de passe | String | Mot de passe pour protéger le classeur. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodProtectWithProtectionTypeStringDemo
    {
        public static void Run()
        {
            Workbook wbk = new Workbook();
            wbk.Protect(ProtectionType.Structure, "password123");
            
            wbk.Save("protected_workbook.xlsx", SaveFormat.Xlsx);
            wbk.Dispose();
        }
    }
}
```

### Voir aussi

* enum [ProtectionType](../../protectiontype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


