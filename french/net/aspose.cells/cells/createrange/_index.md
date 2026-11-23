---
title: "Cells.CreateRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Crée un objet Range à partir d’une plage de cellules"
type: docs
url: /fr/net/aspose.cells/cells/createrange/
---
## CreateRange(string, string) {#createrange_3}

Crée un objet [`Range`](../../range/) à partir d’une plage de cellules.

```csharp
public Range CreateRange(string upperLeftCell, string lowerRightCell)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| upperLeftCell | String | Nom de la cellule en haut à gauche. |
| lowerRightCell | String | Nom de la cellule en bas à droite. |

### Valeur de retour

Un objet [`Range`](../../range/)

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCreateRangeWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Créez une plage de A1 à A2
            Aspose.Cells.Range range = cells.CreateRange("A1", "A2");
            range.Name = "MyRange";
            
            // Définissez les valeurs dans la plage
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            
            // Utilisez la plage dans une formule
            cells["B1"].Formula = "=SUM(MyRange)";
            
            // Calculer la formule
            workbook.CalculateFormula();
            
            Console.WriteLine("Sum of MyRange (A1:A2) is: " + cells["B1"].IntValue);
        }
    }
}
```

### Voir aussi

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateRange(int, int, int, int) {#createrange_1}

Crée un objet [`Range`](../../range/) à partir d’une plage de cellules.

```csharp
public Range CreateRange(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | Première ligne de cette plage |
| firstColumn | Int32 | Première colonne de cette plage |
| totalRows | Int32 | Nombre de lignes |
| totalColumns | Int32 | Nombre de colonnes |

### Valeur de retour

Un objet [`Range`](../../range/)

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCreateRangeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Créez la plage source (ligne de départ 2, colonne 2 avec 3 lignes et 4 colonnes)
            Aspose.Cells.Range rangeSrc = cells.CreateRange(2, 2, 3, 4);

            // Remplir la plage source avec des données d'exemple
            for (int i = 0; i < rangeSrc.RowCount; i++)
            {
                for (int j = 0; j < rangeSrc.ColumnCount; j++)
                {
                    rangeSrc[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Créer la plage de destination (ligne de départ 8, colonne 0 avec les mêmes dimensions)
            Aspose.Cells.Range rangeDest = cells.CreateRange(8, 0, 3, 4);

            // Copier les valeurs de la source vers la destination
            rangeDest.CopyValue(rangeSrc);

            // Enregistrez le classeur
            workbook.Save("CreateRangeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateRange(string) {#createrange_2}

Crée un objet [`Range`](../../range/) à partir d'une adresse de la plage.

```csharp
public Range CreateRange(string address)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| address | String | L'adresse de la plage. |

### Valeur de retour

Un objet [`Range`](../../range/)

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCreateRangeWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une plage à l'aide d'une adresse sous forme de chaîne
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:D4");

            // Remplir la plage avec des données
            for (int i = 0; i < range.RowCount; i++)
            {
                for (int j = 0; j < range.ColumnCount; j++)
                {
                    range[i, j].PutValue($"Cell {i},{j}");
                }
            }

            // Créer une autre plage dans une nouvelle feuille de calcul
            workbook.Worksheets.Add();
            Worksheet worksheet2 = workbook.Worksheets[1];
            Aspose.Cells.Range range2 = worksheet2.Cells.CreateRange("A1:C3");

            // Copier des données entre les plages
            range2.Copy(range);

            // Enregistrez le classeur
            workbook.Save("CreateRangeWithStringDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateRange(int, int, bool) {#createrange}

Crée un objet [`Range`](../../range/) à partir de lignes de cellules ou de colonnes de cellules.

```csharp
public Range CreateRange(int firstIndex, int number, bool isVertical)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| firstIndex | Int32 | Indice de la première ligne ou indice de la première colonne, basé sur zéro. |
| nombre | Int32 | Nombre total de lignes ou de colonnes, basé sur un. |
| isVertical | Boolean | Vrai - Plage créée à partir de colonnes de cellules. Faux - Plage créée à partir de lignes de cellules. |

### Valeur de retour

Un objet [`Range`](../../range/).

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCreateRangeWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Créer une plage commençant à la cellule A1 (0,0) avec 5 lignes et 3 colonnes
            Aspose.Cells.Range range = cells.CreateRange(0, 0, true);

            // Remplir la plage avec quelques données
            for (int i = 0; i < range.RowCount; i++)
            {
                for (int j = 0; j < range.ColumnCount; j++)
                {
                    range[i, j].PutValue($"Row {i}, Col {j}");
                }
            }

            // Enregistrez le classeur
            workbook.Save("CreateRangeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


