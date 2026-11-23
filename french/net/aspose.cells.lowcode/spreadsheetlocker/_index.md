---
title: "Classe SpreadsheetLocker"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.LowCode.SpreadsheetLocker. API low‑code pour verrouiller le fichier de feuille de calcul"
type: docs
url: /fr/net/aspose.cells.lowcode/spreadsheetlocker/
---
## SpreadsheetLocker class

API low-code pour verrouiller le fichier de feuille de calcul.

```csharp
public class SpreadsheetLocker
```

## Méthodes

| Nom | Description |
| --- | --- |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process)(LowCodeLoadOptions, LowCodeSaveOptions, AbstractLowCodeProtectionProvider) | Verrouille le fichier de feuille de calcul avec les paramètres spécifiés. |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process_1)(LowCodeLoadOptions, LowCodeSaveOptions, string, string) | Verrouille le fichier de feuille de calcul avec les paramètres spécifiés. |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process_3)(string, string, string, string) | Verrouille le fichier de feuille de calcul avec les paramètres spécifiés. |
| static [Process](../../aspose.cells.lowcode/spreadsheetlocker/process/#process_2)(LowCodeLoadOptions, LowCodeSaveOptions, string, string, string, ProtectionType) | Verrouille le fichier de feuille de calcul avec les paramètres spécifiés. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassSpreadsheetLockerDemo
    {
        public static void Run()
        {
            // Utilisez SpreadsheetLocker pour protéger le classeur
            SpreadsheetLocker.Process("template.xlsx", "locked.xlsx", "mypassword", "mypassword");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


