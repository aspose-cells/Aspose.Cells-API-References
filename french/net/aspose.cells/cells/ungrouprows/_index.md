---
title: "Cells.UngroupRows"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Dégroupe les lignes"
type: docs
url: /fr/net/aspose.cells/cells/ungrouprows/
---
## UngroupRows(int, int, bool) {#ungrouprows_1}

Dégroupe les lignes.

```csharp
public void UngroupRows(int firstIndex, int lastIndex, bool isAll)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| firstIndex | Int32 | Le premier indice de ligne à dégrouper. |
| lastIndex | Int32 | Le dernier indice de ligne à dégrouper. |
| isAll | Boolean | True, supprime toutes les informations groupées.Sinon, supprime les informations du groupe externe. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodUngroupRowsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des groupements de lignes imbriqués à des fins de démonstration
            worksheet.Cells.GroupRows(5, 7);  // First level grouping
            worksheet.Cells.GroupRows(5, 7);  // Second level grouping

            try
            {
                // Dégrouper tous les niveaux des lignes 5-7
                worksheet.Cells.UngroupRows(5, 7, true);

                Console.WriteLine("Rows 5-7 successfully ungrouped with all levels removed");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UngroupRows: {ex.Message}");
            }

            // Enregistrer le classeur modifié
            workbook.Save("UngroupRowsWithBooleanDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## UngroupRows(int, int) {#ungrouprows}

Dégroupe les lignes.

```csharp
public void UngroupRows(int firstIndex, int lastIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| firstIndex | Int32 | Le premier indice de ligne à dégrouper. |
| lastIndex | Int32 | Le dernier indice de ligne à dégrouper. |

### Remarques

Supprime uniquement les informations du groupe externe.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUngroupRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Remplissez quelques données
            for (int i = 0; i < 6; i++)
            {
                cells[i, 0].PutValue($"Row {i}");
            }

            // Grouper les lignes 1 à 3 (indice basé sur 0)
            cells.GroupRows(1, 3, true);

            Console.WriteLine("Rows grouped from index 1 to 3");

            // Dégrouper les mêmes lignes
            cells.UngroupRows(1, 3);

            Console.WriteLine("Rows ungrouped from index 1 to 3");

            // Enregistrez le classeur
            workbook.Save("UngroupRowsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


