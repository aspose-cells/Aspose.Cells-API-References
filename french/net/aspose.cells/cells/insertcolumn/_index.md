---
title: "Cells.InsertColumn"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Insère une nouvelle colonne dans la feuille de calcul"
type: docs
url: /fr/net/aspose.cells/cells/insertcolumn/
---
## InsertColumn(int, bool) {#insertcolumn_1}

Insère une nouvelle colonne dans la feuille de calcul.

```csharp
public void InsertColumn(int columnIndex, bool updateReference)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Index de colonne. |
| updateReference | Boolean | Indique si les références dans d'autres feuilles de calcul seront mises à jour. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertColumnWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Remplissez quelques données d'exemple dans la colonne 0
            Cells cells = sheet.Cells;
            for (int i = 0; i < 5; i++)
            {
                cells[i, 0].PutValue($"Original {i}");
            }

            // Insérez une nouvelle colonne à l'index 1 et décalez les colonnes vers la droite
            cells.InsertColumn(1, true);

            // Copiez les données de la colonne 0 vers la nouvelle colonne 1
            cells.CopyColumn(cells, 0, 1);

            // Enregistrez le classeur
            workbook.Save("InsertColumnDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertColumn(int) {#insertcolumn}

Insère une nouvelle colonne dans la feuille de calcul.

```csharp
public void InsertColumn(int columnIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Index de colonne. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertColumnWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet sheet = workbook.Worksheets[0];
            
            // Obtenez la collection de cellules
            Cells cells = sheet.Cells;
            
            // Insérez des données dans les cellules à des fins de démonstration
            cells["A1"].PutValue("Column A");
            cells["B1"].PutValue("Column B");
            cells["C1"].PutValue("Column C");
            
            // Insérez une nouvelle colonne à l'index 1 (deviendra la nouvelle colonne B)
            cells.InsertColumn(1);
            
            // Vérifiez en insérant des données dans la nouvelle colonne
            cells["B1"].PutValue("New Column");
            
            // Enregistrez le classeur
            workbook.Save("InsertColumnDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


