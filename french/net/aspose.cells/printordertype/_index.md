---
title: "Enum PrintOrderType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.PrintOrderType enum. Représente les constantes d'ordre d'impression"
type: docs
url: /fr/net/aspose.cells/printordertype/
---
## PrintOrderType enumeration

Représente les constantes d'ordre d'impression.

```csharp
public enum PrintOrderType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| DownThenOver | `0` | Vers le bas, puis à droite |
| OverThenDown | `1` | Vers la droite, puis vers le bas |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PrintOrderTypeDemo
    {
        public static void PrintOrderTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accéder à l'objet PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // Définir l'ordre d'impression sur DownThenOver
            pageSetup.Order = PrintOrderType.DownThenOver;

            // Définir d'autres propriétés de configuration de page pour la démonstration
            pageSetup.PrintArea = "A1:D10";
            pageSetup.PrintTitleRows = "$1:$1";
            pageSetup.PrintTitleColumns = "$A:$A";
            pageSetup.CenterHorizontally = true;
            pageSetup.CenterVertically = true;

            // Enregistrez le classeur
            workbook.Save("PrintOrderTypeExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


