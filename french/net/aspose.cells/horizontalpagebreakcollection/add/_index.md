---
title: "HorizontalPageBreakCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode HorizontalPageBreakCollection. Ajoute un saut de page horizontal à la collection"
type: docs
url: /fr/net/aspose.cells/horizontalpagebreakcollection/add/
---
## Add(int, int, int) {#add_2}

Ajoute un saut de page horizontal à la collection.

```csharp
public int Add(int row, int startColumn, int endColumn)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | Indice de ligne, basé sur zéro. |
| startColumn | Int32 | Indice de colonne de départ, basé sur zéro. |
| endColumn | Int32 | Indice de colonne de fin, basé sur zéro. |

### Valeur de retour

[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.

### Remarques

Cette méthode est utilisée pour ajouter un saut de page horizontal dans une zone d'impression.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakCollectionMethodAddWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Démontrer la méthode Add avec les paramètres (Int32, Int32, Int32)
            worksheet.HorizontalPageBreaks.Add(10, 1, 5);
            
            workbook.Save("HorizontalPageBreakExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int) {#add}

Ajoute un saut de page horizontal à la collection.

```csharp
public int Add(int row)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | Indice de ligne de cellule, à base zéro. |

### Valeur de retour

[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.

### Remarques

Le saut de page est ajouté en haut à gauche de la cellule. Veuillez définir un saut de page horizontal et un saut de page vertical simultanément.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakCollectionMethodAddWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des sauts de page horizontaux en utilisant le paramètre Int32
            worksheet.HorizontalPageBreaks.Add(5);
            worksheet.HorizontalPageBreaks.Add(10);
            
            workbook.Save("HorizontalPageBreakExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int) {#add_1}

Ajoute un saut de page horizontal à la collection.

```csharp
public int Add(int row, int column)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | Indice de ligne de cellule, à base zéro. |
| column | Int32 | Indice de colonne de cellule, à base zéro. |

### Valeur de retour

[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.

### Remarques

Le saut de page est ajouté en haut à gauche de la cellule. Veuillez définir un saut de page horizontal et un saut de page vertical simultanément.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour créer plusieurs lignes
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }

            // Ajouter des sauts de page horizontaux à des lignes spécifiques
            worksheet.HorizontalPageBreaks.Add(9, 0);  // Page break after row 9
            worksheet.HorizontalPageBreaks.Add(19, 0); // Page break after row 19
            worksheet.HorizontalPageBreaks.Add(29, 0); // Page break after row 29

            // Enregistrez le classeur
            workbook.Save("HorizontalPageBreaksDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_3}

Ajoute un saut de page horizontal à la collection.

```csharp
public int Add(string cellName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cellName | String | Nom de la cellule. |

### Valeur de retour

[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.

### Remarques

Le saut de page est ajouté en haut à gauche de la cellule. Veuillez définir un saut de page horizontal et un saut de page vertical simultanément.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter un saut de page horizontal à la ligne 4 (D5 est la ligne 4 dans l'index basé sur zéro)
            worksheet.HorizontalPageBreaks.Add("D5");
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


