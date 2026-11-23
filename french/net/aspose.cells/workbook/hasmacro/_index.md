---
title: "Workbook.HasMacro"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Workbook. Indique si cette feuille de calcul contient une macro/VBA"
type: docs
url: /fr/net/aspose.cells/workbook/hasmacro/
---
## Workbook.HasMacro property

Indique si cette feuille de calcul contient des macros/VBA.

```csharp
public bool HasMacro { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyHasMacroDemo
    {
        public static void Run()
        {
            // Créer un classeur avec macro en chargeant un fichier modèle
            Workbook workbookWithMacro = new Workbook("sample_with_macro.xlsm");
            Console.WriteLine("Workbook with macro - HasMacro: " + workbookWithMacro.HasMacro);

            // Créer un classeur sans macro
            Workbook workbookWithoutMacro = new Workbook();
            Console.WriteLine("Workbook without macro - HasMacro: " + workbookWithoutMacro.HasMacro);
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


