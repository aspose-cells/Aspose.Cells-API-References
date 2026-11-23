---
title: "Classe UnionRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.UnionRange. Représente une plage d'union"
type: docs
url: /fr/net/aspose.cells/unionrange/
---
## UnionRange class

Représente une plage d'union.

```csharp
public class UnionRange : IEnumerable
```

## Propriétés

| Nom | Description |
| --- | --- |
| [CellCount](../../aspose.cells/unionrange/cellcount/) { get; } | Obtient le nombre total de cellules dans la plage. |
| [ColumnCount](../../aspose.cells/unionrange/columncount/) { get; } | Obtient le nombre de lignes dans la plage. |
| [FirstColumn](../../aspose.cells/unionrange/firstcolumn/) { get; } | Obtient l'index de la première colonne de la plage. |
| [FirstRow](../../aspose.cells/unionrange/firstrow/) { get; } | Obtient l'index de la première ligne de la plage. |
| [HasRange](../../aspose.cells/unionrange/hasrange/) { get; } | Indique si cela possède une plage. |
| [Hyperlinks](../../aspose.cells/unionrange/hyperlinks/) { get; } | Obtient tous les hyperliens dans la plage. |
| [Name](../../aspose.cells/unionrange/name/) { get; set; } | Obtient ou définit le nom de la plage. |
| [RangeCount](../../aspose.cells/unionrange/rangecount/) { get; } | Obtient le nombre de plages. |
| [Ranges](../../aspose.cells/unionrange/ranges/) { get; } | Obtient toutes les plages d'union. |
| [RefersTo](../../aspose.cells/unionrange/refersto/) { get; } | Obtient la référence de la plage. |
| [RowCount](../../aspose.cells/unionrange/rowcount/) { get; } | Obtient le nombre de lignes dans la plage. |
| [Value](../../aspose.cells/unionrange/value/) { get; set; } | Obtient et définit les valeurs de la plage. |

## Méthodes

| Nom | Description |
| --- | --- |
| [ApplyStyle](../../aspose.cells/unionrange/applystyle/)(Style, StyleFlag) | Applique des formats à une plage entière. |
| [Copy](../../aspose.cells/unionrange/copy/)(UnionRange, PasteOptions) | Copie la plage avec les options de collage spécial. |
| [GetEnumerator](../../aspose.cells/unionrange/getenumerator/)() | Obtient l'énumérateur des cellules de cette `Range`. |
| [Intersect](../../aspose.cells/unionrange/intersect/#intersect)(Range[]) | Intersecte une autre plage. |
| [Intersect](../../aspose.cells/unionrange/intersect/#intersect_2)(string) | Intersecte une autre plage. |
| [Intersect](../../aspose.cells/unionrange/intersect/#intersect_1)(UnionRange) | Intersecte une autre plage. |
| [Merge](../../aspose.cells/unionrange/merge/)() | Combine une plage de cellules en une seule cellule. |
| [PutValue](../../aspose.cells/unionrange/putvalue/)(string, bool, bool) | Insère une valeur dans la plage, le cas échéant la valeur sera convertie en un autre type de données et le format numérique de la cellule sera réinitialisé. |
| [SetOutlineBorders](../../aspose.cells/unionrange/setoutlineborders/#setoutlineborders)(CellBorderType, Color) | Définit les bordures extérieures autour d'une plage de cellules avec le même style et la même couleur de bordure. |
| [SetOutlineBorders](../../aspose.cells/unionrange/setoutlineborders/#setoutlineborders_1)(CellBorderType[], Color[]) | Définit les bordures extérieures autour d'une plage de cellules. |
| [SetStyle](../../aspose.cells/unionrange/setstyle/)(Style) | Définit le style de la plage. |
| [Union](../../aspose.cells/unionrange/union/#union)(Range[]) | Fusionne les plages. |
| [Union](../../aspose.cells/unionrange/union/#union_2)(string) | Fusionne une autre plage. |
| [Union](../../aspose.cells/unionrange/union/#union_1)(UnionRange) | Fusionne une autre plage. |
| [UnMerge](../../aspose.cells/unionrange/unmerge/)() | Démarque les cellules fusionnées de cette plage. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassUnionRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crée une plage d'union en utilisant l'API correcte
            UnionRange unionRange = workbook.Worksheets.CreateUnionRange("A1:A10,C1:C10", 0);
            
            // Définit la valeur pour l'ensemble de la plage d'union
            unionRange.Value = "Test";
            
            // Applique le style à la plage d'union
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            unionRange.ApplyStyle(style, new StyleFlag { All = true });
            
            // Enregistrez le classeur
            workbook.Save("UnionRangeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


