---
title: "Enum LookAtType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.LookAtType enum. Représente le type de recherche"
type: docs
url: /fr/net/aspose.cells/lookattype/
---
## LookAtType enumeration

Représente le type de recherche.

```csharp
public enum LookAtType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Contains | `0` | La valeur de la cellule contient l'objet recherché. |
| StartWith | `1` | La valeur de la cellule commence par l'objet recherché. |
| EndWith | `2` | La valeur de la cellule se termine par l'objet recherché. |
| EntireContent | `3` | La valeur de la cellule est identique à l'objet recherché. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LookAtTypeDemo
    {
        public static void LookAtTypeExample()
        {
            // Instancier l'objet classeur
            Workbook workbook = new Workbook("LookAtTypeExample_original.xlsx");

            // Obtenir la collection Cells
            Cells cells = workbook.Worksheets[0].Cells;

            // Instancier l'objet FindOptions
            FindOptions findOptions = new FindOptions();

            // Créer une zone Cells
            CellArea ca = new CellArea();
            ca.StartRow = 8;
            ca.StartColumn = 2;
            ca.EndRow = 17;
            ca.EndColumn = 13;

            // Définir la zone de cellules pour les options de recherche
            findOptions.SetRange(ca);

            // Définir les propriétés de recherche
            findOptions.SearchBackward = false;
            findOptions.SearchOrderByRows = true;
            findOptions.LookInType = LookInType.Values;

            // Définir LookAtType sur Contains
            findOptions.LookAtType = LookAtType.Contains;

            // Trouver la cellule avec une valeur spécifique
            Cell cell = cells.Find("searchValue", null, findOptions);

            if (cell != null)
            {
                Console.WriteLine($"Cell found at row {cell.Row}, column {cell.Column}");
            }
            else
            {
                Console.WriteLine("Cell not found.");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


