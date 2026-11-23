---
title: "Classe FindOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.FindOptions. Représente les options de recherche"
type: docs
url: /fr/net/aspose.cells/findoptions/
---
## FindOptions class

Représente les options de recherche.

```csharp
public class FindOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [FindOptions](findoptions/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [CaseSensitive](../../aspose.cells/findoptions/casesensitive/) { get; set; } | Indique si la chaîne recherchée est sensible à la casse. |
| [ConvertNumericData](../../aspose.cells/findoptions/convertnumericdata/) { get; set; } | Obtient ou définit une valeur qui indique si la conversion de la chaîne recherchée en données numériques est effectuée. |
| [IsCaseSensitive](../../aspose.cells/findoptions/iscasesensitive/) { get; set; } | (**Obsolete.**) Indique si la chaîne recherchée est sensible à la casse. |
| [IsRangeSet](../../aspose.cells/findoptions/israngeset/) { get; } | Indique si la plage recherchée est définie. |
| [LookAtType](../../aspose.cells/findoptions/lookattype/) { get; set; } | Regarder le type. |
| [LookInType](../../aspose.cells/findoptions/lookintype/) { get; set; } | Regarder dans le type. |
| [RegexKey](../../aspose.cells/findoptions/regexkey/) { get; set; } | Indique si la clé recherchée est une expression régulière. Si vrai, la clé recherchée sera prise comme expression régulière et analysée. Sinon, la clé sera analysée selon les règles de MS Excel. |
| [SearchBackward](../../aspose.cells/findoptions/searchbackward/) { get; set; } | Indique si la recherche doit se faire en arrière pour les cellules. |
| [SearchNext](../../aspose.cells/findoptions/searchnext/) { get; set; } | (**Obsolète.**) Ordre de recherche. Vrai : rechercher le suivant. Faux : rechercher le précédent. |
| [SearchOrderByRows](../../aspose.cells/findoptions/searchorderbyrows/) { get; set; } | Indique si l'ordre de recherche est par lignes ou par colonnes. |
| [Style](../../aspose.cells/findoptions/style/) { get; set; } | Le format à rechercher. |
| [ValueTypeSensitive](../../aspose.cells/findoptions/valuetypesensitive/) { get; set; } | Indique si le type de valeur de la cellule recherchée doit être le même que la clé recherchée. |

## Méthodes

| Nom | Description |
| --- | --- |
| [GetRange](../../aspose.cells/findoptions/getrange/)() | Obtient et définit la plage recherchée. |
| [SetRange](../../aspose.cells/findoptions/setrange/)(CellArea) | Définit la plage recherchée. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FindOptionsDemo
    {
        public static void FindOptionsExample()
        {
            // Instancier l'objet classeur
            Workbook workbook = new Workbook("FindOptionsExample_original.xlsx");

            // Obtenir la collection Cells
            Cells cells = workbook.Worksheets[0].Cells;

            // Instancier l'objet FindOptions
            FindOptions findOptions = new FindOptions();

            // Créer une zone Cells
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.StartColumn = 0;
            ca.EndRow = 5;
            ca.EndColumn = 5;

            // Définir la zone de cellules pour les options de recherche
            findOptions.SetRange(ca);

            // Définir les propriétés de recherche
            findOptions.SearchBackward = false;
            findOptions.SearchOrderByRows = true;
            findOptions.LookInType = LookInType.Values;

            // Trouve la cellule avec la valeur 0
            Cell cell = cells.Find(0, null, findOptions);

            if (cell != null)
            {
                Console.WriteLine("Cell found at: " + cell.Name);
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


