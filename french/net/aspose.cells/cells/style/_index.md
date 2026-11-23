---
title: "Cells.Style"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cells. Obtient et définit le style par défaut de la feuille de calcul"
type: docs
url: /fr/net/aspose.cells/cells/style/
---
## Cells.Style property

Obtient et définit le style par défaut de la feuille de calcul.

```csharp
public Style Style { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStyleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définissez une valeur dans la cellule A1
            Cell cell = cells["A1"];
            cell.PutValue(43368); // This represents the date 2018-09-25

            // Obtenez le style par défaut et modifiez son format
            Style style = cells.Style;
            style.CultureCustom = "yyyymmdd!y";
            
            // Appliquer le style modifié à la cellule
            cell.SetStyle(style);

            // Affichez la valeur de chaîne formatée
            Console.WriteLine("Formatted value: " + cell.StringValue);
        }
    }
}
```

### Voir aussi

* class [Style](../../style/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


