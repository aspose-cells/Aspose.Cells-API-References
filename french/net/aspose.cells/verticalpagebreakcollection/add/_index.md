---
title: "VerticalPageBreakCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode VerticalPageBreakCollection. Ajoute un saut de page vertical à la collection"
type: docs
url: /fr/net/aspose.cells/verticalpagebreakcollection/add/
---
## Add(int, int, int) {#add_2}

Ajoute un saut de page vertical à la collection.

```csharp
public int Add(int startRow, int endRow, int column)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Indice de ligne de départ, basé sur zéro. |
| endRow | Int32 | Indice de ligne de fin, basé sur zéro. |
| column | Int32 | Indice de colonne, à base zéro. |

### Valeur de retour

[`VerticalPageBreak`](../../verticalpagebreak/) object index.

### Remarques

Cette méthode est utilisée pour ajouter un saut de page vertical dans une zone d'impression.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakCollectionMethodAddWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            VerticalPageBreakCollection verticalPageBreaks = worksheet.VerticalPageBreaks;
            
            // Démontrer Add avec les paramètres (Int32, Int32, Int32)
            verticalPageBreaks.Add(0, 10, 2); // From row 0 to 10 at column 2
            
            // Exemples supplémentaires pour le contexte
            verticalPageBreaks.Add(4); // At column 4
            verticalPageBreaks.Add(5, 3); // At row 5, column 3

            Console.WriteLine("Vertical Page Breaks:");
            for (int i = 0; i < verticalPageBreaks.Count; i++)
            {
                VerticalPageBreak vpb = verticalPageBreaks[i];
                Console.WriteLine($"{i}: StartRow={vpb.StartRow}, EndRow={vpb.EndRow}, Column={vpb.Column}");
            }

            workbook.Save("VerticalPageBreakDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int) {#add}

Ajoute un saut de page vertical à la collection.

```csharp
public int Add(int column)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| column | Int32 | Indice de colonne de cellule, à base zéro. |

### Valeur de retour

[`VerticalPageBreak`](../../verticalpagebreak/) object index.

### Remarques

Le saut de page est ajouté en haut à gauche de la cellule. Veuillez définir un saut de page horizontal et un saut de page vertical simultanément.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakCollectionMethodAddWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            VerticalPageBreakCollection verticalPageBreaks = worksheet.VerticalPageBreaks;

            // Démontrer la méthode Add avec le paramètre Int32
            verticalPageBreaks.Add(4); // Add vertical page break at column 4

            // Imprimer les détails du saut de page ajouté
            VerticalPageBreak vpb = verticalPageBreaks[0];
            Console.WriteLine($"Vertical Page Break: StartRow = {vpb.StartRow}, EndRow = {vpb.EndRow}, Column = {vpb.Column}");

            workbook.Save("VerticalPageBreakCollectionExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int) {#add_1}

Ajoute un saut de page vertical à la collection.

```csharp
public int Add(int row, int column)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | Indice de ligne de cellule, à base zéro. |
| column | Int32 | Indice de colonne de cellule, à base zéro. |

### Valeur de retour

[`VerticalPageBreak`](../../verticalpagebreak/) object index.

### Remarques

Le saut de page est ajouté en haut à gauche de la cellule. Veuillez définir un saut de page horizontal et un saut de page vertical simultanément.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtenir la collection des sauts de page verticaux
            VerticalPageBreakCollection vPageBreaks = worksheet.VerticalPageBreaks;

            // Ajouter des sauts de page verticaux à différentes positions de colonne
            vPageBreaks.Add(0, 5);  // Add page break after column 5
            vPageBreaks.Add(0, 10); // Add page break after column 10
            vPageBreaks.Add(0, 15); // Add page break after column 15

            // Ajouter des données d'exemple pour visualiser les sauts de page
            for (int i = 0; i < 20; i++)
            {
                worksheet.Cells[0, i].PutValue($"Column {i + 1}");
            }

            // Enregistrez le classeur
            workbook.Save("VerticalPageBreaksDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_3}

Ajoute un saut de page vertical à la collection.

```csharp
public int Add(string cellName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cellName | String | Nom de la cellule. |

### Valeur de retour

[`VerticalPageBreak`](../../verticalpagebreak/) object index.

### Remarques

Le saut de page est ajouté en haut à gauche de la cellule. Veuillez définir un saut de page horizontal et un saut de page vertical simultanément.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.VerticalPageBreaks.Add("G5");
            
            VerticalPageBreak vpb = worksheet.VerticalPageBreaks[0];
            Console.WriteLine("Start Row: " + vpb.StartRow);
            Console.WriteLine("End Row: " + vpb.EndRow);
            Console.WriteLine("Column: " + vpb.Column);
        }
    }
}
```

### Voir aussi

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


