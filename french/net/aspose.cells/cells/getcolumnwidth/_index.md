---
title: "Cells.GetColumnWidth"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Obtient la largeur de la colonne"
type: docs
url: /fr/net/aspose.cells/cells/getcolumnwidth/
---
## GetColumnWidth(int, bool, CellsUnitType) {#getcolumnwidth_1}

Obtient la largeur de la colonne.

```csharp
public double GetColumnWidth(int column, bool isOriginal, CellsUnitType unitType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| column | Int32 | L'index de colonne. |
| isOriginal | Boolean | Indique si la largeur originale est obtenue. |
| unitType | CellsUnitType |  |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetColumnWidthWithInt32BooleanCellsUnitTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définir la largeur de la colonne 1 (indice basé sur 0)
            cells.SetColumnWidth(0, 20);

            // Obtenir la largeur de la colonne dans différentes unités et modes
            double widthInPixels = cells.GetColumnWidth(0, true, CellsUnitType.Pixel);
            double widthInPoints = cells.GetColumnWidth(0, true, CellsUnitType.Point);
            double defaultWidth = cells.GetColumnWidth(0, false, CellsUnitType.Pixel);

            Console.WriteLine("Column width in pixels: " + widthInPixels);
            Console.WriteLine("Column width in points: " + widthInPoints);
            Console.WriteLine("Default column width: " + defaultWidth);
        }
    }
}
```

### Voir aussi

* enum [CellsUnitType](../../cellsunittype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetColumnWidth(int) {#getcolumnwidth}

Obtient la largeur (en unités de caractères) de la colonne spécifiée en vue normale

```csharp
public double GetColumnWidth(int column)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| column | Int32 | Indice de colonne |

### Valeur de retour

Largeur de la colonne. Pour les feuilles de calcul, la largeur de la colonne est mesurée en nombre de caractères de la largeur maximale d'un chiffre des nombres 0~9 tels qu'ils sont rendus dans la police du style normal.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetColumnWidthWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définir la largeur de la colonne pour l'indice de colonne 255
            cells.SetColumnWidth(255, 20.86);

            // Obtenir et afficher la largeur de la colonne
            double columnWidth = cells.GetColumnWidth(255);
            Console.WriteLine("Column width at index 255: " + columnWidth);
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


