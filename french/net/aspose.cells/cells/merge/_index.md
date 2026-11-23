---
title: "Cells.Merge"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Fusionne une plage de cellules spécifiée en une seule cellule"
type: docs
url: /fr/net/aspose.cells/cells/merge/
---
## Merge(int, int, int, int) {#merge}

Fusionne une plage de cellules spécifiée en une seule cellule.

```csharp
public void Merge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | Première ligne de cette plage (index zéro) |
| firstColumn | Int32 | Première colonne de cette plage (index zéro) |
| totalRows | Int32 | Nombre de lignes (indexé à 1) |
| totalColumns | Int32 | Nombre de colonnes (indexé à 1) |

### Remarques

Faites référence à la cellule fusionnée via l'adresse de la cellule en haut à gauche de la plage.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodMergeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Placez des valeurs dans les cellules pour démontrer la fusion
            cells[0, 0].PutValue("Merged Area");
            cells[5, 5].PutValue("Not Merged");

            // Fusionnez les cellules à partir de la ligne 0, colonne 0 en couvrant 3 lignes et 2 colonnes
            cells.Merge(0, 0, 3, 2);

            // Enregistrez le classeur
            workbook.Save("MergeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Merge(int, int, int, int, bool) {#merge_1}

Fusionne une plage de cellules spécifiée en une seule cellule.

```csharp
public void Merge(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    bool mergeConflict)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | Première ligne de cette plage (index zéro) |
| firstColumn | Int32 | Première colonne de cette plage (index zéro) |
| totalRows | Int32 | Nombre de lignes (indexé à 1) |
| totalColumns | Int32 | Nombre de colonnes (indexé à 1) |
| mergeConflict | Boolean | Fusion de plages fusionnées en conflit. |

### Remarques

Faites référence à la cellule fusionnée via l'adresse de la cellule en haut à gauche de la plage. Si mergeConflict est vrai et que la plage fusionnée entre en conflit avec d'autres cellules fusionnées, les autres cellules fusionnées seront automatiquement supprimées.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodMergeWithInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fusionnez les cellules de la ligne 3, colonne 4 (D3) à la ligne 7, colonne 5 (E7) - 5 lignes et 2 colonnes
            worksheet.Cells.Merge(3, 4, 5, 2, true);
            
            // Enregistrez le classeur
            workbook.Save("MergeDemoOutput.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Merge(int, int, int, int, bool, bool) {#merge_2}

Fusionne une plage de cellules spécifiée en une seule cellule.

```csharp
public void Merge(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    bool checkConflict, bool mergeConflict)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | Première ligne de cette plage (index zéro) |
| firstColumn | Int32 | Première colonne de cette plage (index zéro) |
| totalRows | Int32 | Nombre de lignes (indexé à 1) |
| totalColumns | Int32 | Nombre de colonnes (indexé à 1) |
| checkConflict | Boolean | Indique si la vérification des cellules fusionnées intersecte d'autres cellules fusionnées |
| mergeConflict | Boolean | Fusion de plages fusionnées en conflit. |

### Remarques

Faites référence à la cellule fusionnée via l'adresse de la cellule en haut à gauche de la plage. Si mergeConflict est vrai et que la plage fusionnée entre en conflit avec d'autres cellules fusionnées, les autres cellules fusionnées seront automatiquement supprimées.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodMergeWithInt32Int32Int32Int32BooleanBooDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Placez des données dans les cellules à fusionner
            cells[0, 1].PutValue("Merged Cell");
            cells[1, 1].PutValue("This will be merged");

            // Fusionnez les cellules sans options (fusion simple)
            cells.Merge(0, 1, 2, 2);
            Console.WriteLine("Cells merged without options");

            // Annulez la fusion d'abord pour démontrer la prochaine fusion
            cells.UnMerge(0, 1, 2, 2);

            // Fusionnez les cellules avec ignoreStyle=false et mergeConflict=true
            cells.Merge(0, 1, 2, 2, false, true);
            Console.WriteLine("Cells merged with ignoreStyle=false and mergeConflict=true");

            // Enregistrez le classeur
            workbook.Save("MergeCellsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


