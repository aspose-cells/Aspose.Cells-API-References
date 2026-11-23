---
title: "Cells.GroupRows"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Regroupe les lignes"
type: docs
url: /fr/net/aspose.cells/cells/grouprows/
---
## GroupRows(int, int, bool) {#grouprows_1}

Regroupe les lignes.

```csharp
public void GroupRows(int firstIndex, int lastIndex, bool isHidden)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| firstIndex | Int32 | Le premier indice de ligne à regrouper. |
| lastIndex | Int32 | Le dernier indice de ligne à regrouper. |
| isHidden | Boolean | Spécifie si les lignes regroupées sont masquées. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGroupRowsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Remplissez quelques données
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue($"Group {i + 1}");
                for (int j = 1; j <= 5; j++)
                {
                    cells[i, j].PutValue($"Data {j}");
                }
            }

            // Regroupez les lignes 1 à 5 (indice basé sur 0) et masquez-les
            cells.GroupRows(1, 5, true);

            // Définir la ligne de résumé sous le groupe
            worksheet.Outline.SummaryRowBelow = false;

            // Enregistrez le classeur
            workbook.Save("GroupRowsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GroupRows(int, int) {#grouprows}

Regroupe les lignes.

```csharp
public void GroupRows(int firstIndex, int lastIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| firstIndex | Int32 | Le premier indice de ligne à regrouper. |
| lastIndex | Int32 | Le dernier indice de ligne à regrouper. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGroupRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Remplir des données d'exemple
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue("Row " + (i + 1));
            }

            // Regroupez les lignes 2 à 5 (indice basé sur zéro)
            cells.GroupRows(1, 4);

            // Enregistrez le classeur
            workbook.Save("GroupRowsExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


