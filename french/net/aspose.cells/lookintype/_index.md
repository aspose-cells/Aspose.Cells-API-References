---
title: "Enum LookInType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.LookInType enum. Représente le type de recherche"
type: docs
url: /fr/net/aspose.cells/lookintype/
---
## LookInType enumeration

Représente le type de recherche dans.

```csharp
public enum LookInType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Formulas | `0` | Recherche l'objet recherché à partir de la formule([`Formula`](../cell/formula/)) si la cellule est une formule, sinon le trouve à partir de la valeur originale de la cellule (identique à OriginalValues). |
| Values | `1` | Recherche l'objet à partir de la valeur originale de la cellule([`Value`](../cell/value/)) et de la valeur formatée([`StringValue`](../cell/stringvalue/)). |
| ValuesExcludeFormulaCell | `2` | Ignore les cellules qui sont des formules. Pour les cellules qui ne sont pas des formules, c'est identique à Values. |
| Comments | `3` | Recherche l'objet uniquement à partir du commentaire de la cellule. Ignore les cellules qui n'ont pas de commentaire. |
| OnlyFormulas | `4` | Ignore les cellules qui ne sont pas des formules. Pour les cellules qui sont des formules, recherche l'objet recherché à partir de la formule([`Formula`](../cell/formula/)). |
| OriginalValues | `5` | Recherche l'objet uniquement à partir de la valeur originale de la cellule. |
| FormattedValues | `6` | Recherche l'objet uniquement à partir de la valeur formatée de la cellule([`StringValue`](../cell/stringvalue/)). |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassLookInTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données et des formules
            worksheet.Cells["A1"].PutValue("Test");
            worksheet.Cells["B1"].Formula = "=A1";
            worksheet.Cells["C1"].PutValue("Contains B1");

            // Trouvez la cellule contenant la formule avec "B1"
            FindOptions options = new FindOptions
            {
                LookInType = LookInType.OnlyFormulas,
                LookAtType = LookAtType.Contains
            };

            Cell foundCell = worksheet.Cells.Find("B1", null, options);

            // Afficher le résultat
            if (foundCell != null)
            {
                Console.WriteLine($"Found cell at row: {foundCell.Row}, column: {foundCell.Column}");
                Console.WriteLine($"Cell value: {foundCell.StringValue}");
                Console.WriteLine($"Cell formula: {foundCell.Formula}");
            }
            else
            {
                Console.WriteLine("Cell not found");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


