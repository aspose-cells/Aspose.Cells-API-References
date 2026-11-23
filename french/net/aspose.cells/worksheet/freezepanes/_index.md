---
title: "Worksheet.FreezePanes"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Worksheet. Gèle les volets à la cellule spécifiée dans la feuille de calcul"
type: docs
url: /fr/net/aspose.cells/worksheet/freezepanes/
---
## FreezePanes(int, int, int, int) {#freezepanes}

Gèle les volets à la cellule spécifiée dans la feuille de calcul.

```csharp
public void FreezePanes(int row, int column, int freezedRows, int freezedColumns)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | Index de ligne. |
| column | Int32 | Index de colonne. |
| freezedRows | Int32 | Nombre de lignes visibles dans le volet supérieur, ne dépassant pas l'index de ligne. |
| freezedColumns | Int32 | Nombre de colonnes visibles dans le volet gauche, ne dépassant pas l'index de colonne. |

### Remarques

L'index de ligne et l'index de colonne ne peuvent pas tous deux être zéro. Le nombre de lignes et le nombre de colonnes ne peuvent pas non plus être tous deux zéro.

Les deux premiers paramètres spécifient la position gelée et les deux derniers paramètres spécifient la zone gelée dans le volet supérieur gauche.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodFreezePanesWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Geler les volets à la ligne 3, colonne 3, avec 3 lignes gelées et 3 colonnes gelées
            worksheet.FreezePanes(3, 3, 3, 3);
            
            // Enregistrez le classeur
            workbook.Save("FreezePanesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## FreezePanes(string, int, int) {#freezepanes_1}

Gèle les volets à la cellule spécifiée dans la feuille de calcul.

```csharp
public void FreezePanes(string cellName, int freezedRows, int freezedColumns)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cellName | String | Nom de la cellule. |
| freezedRows | Int32 | Nombre de lignes visibles dans le volet supérieur, ne dépassant pas l'index de ligne. |
| freezedColumns | Int32 | Nombre de colonnes visibles dans le volet gauche, ne dépassant pas l'index de colonne. |

### Remarques

L'index de ligne et l'index de colonne ne peuvent pas tous deux être zéro. Le nombre de lignes et le nombre de colonnes ne peuvent pas non plus être tous deux zéro.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodFreezePanesWithStringInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Geler les volets à "C3" avec 3 lignes gelées et 3 colonnes gelées
            worksheet.FreezePanes("C3", 3, 3);

            // Enregistrez le classeur
            workbook.Save("FreezePanesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


