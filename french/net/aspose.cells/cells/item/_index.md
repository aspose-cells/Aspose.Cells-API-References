---
title: "Cells.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cells. Obtient l'élément Cell à l'indice de ligne et de colonne de cellule spécifiés"
type: docs
url: /fr/net/aspose.cells/cells/item/
---
## Cells indexer (1 of 2)

Obtient l'élément [`Cell`](../../cell/) à l'index de ligne et de colonne de cellule spécifié.

```csharp
public Cell this[int row, int column] { get; }
```

| Paramètre | Description |
| --- | --- |
| ligne | Index de ligne. |
| column | Index de colonne. |

### Valeur de retour

L'objet [`Cell`](../../cell/).

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Utilisation de la propriété Item pour accéder et modifier les cellules
            cells[0, 0].PutValue("Hello");
            cells[1, 0].PutValue("World");
            
            // Utilisation de la propriété Style via Cells
            Style style1 = cells[0, 0].GetStyle();
            style1.Font.IsBold = true;
            cells[0, 0].SetStyle(style1);

            Style style2 = cells[1, 0].GetStyle();
            style2.Font.Color = System.Drawing.Color.Red;
            cells[1, 0].SetStyle(style2);

            // Enregistrez le classeur
            workbook.Save("CellsPropertyItemDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Cells indexer (2 of 2)

Obtient l'élément [`Cell`](../../cell/) au nom de cellule spécifié.

```csharp
public Cell this[string cellName] { get; }
```

| Paramètre | Description |
| --- | --- |
| cellName | Nom de cellule, incluant sa lettre de colonne et son numéro de ligne, par exemple A5. |

### Valeur de retour

Un objet [`Cell`](../../cell/)

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyItemDemo1
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accéder à la collection de cellules
            Cells cells = worksheet.Cells;
            
            // Définir des valeurs en utilisant la propriété Item
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            
            // Définir des valeurs dans une plage en utilisant la propriété Item
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(30);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(25);
            
            // Accéder et modifier les propriétés de cellule en utilisant Item
            Cell cell = cells["B1"];
            Style style = cell.GetStyle();
            style.Font.IsBold = true;
            cell.SetStyle(style);
            
            // Enregistrez le classeur
            workbook.Save("CellsPropertyItemDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


