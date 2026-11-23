---
title: "Cells.ClearRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Efface le contenu et le formatage d’une plage"
type: docs
url: /fr/net/aspose.cells/cells/clearrange/
---
## ClearRange(CellArea) {#clearrange}

Efface le contenu et le formatage d'une plage.

```csharp
public void ClearRange(CellArea range)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| plage | CellArea | Plage à effacer. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodClearRangeWithCellAreaDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplir les cellules avec des données d'exemple
            for (int row = 0; row <= 2; row++)
            {
                for (int col = 0; col <= 2; col++)
                {
                    worksheet.Cells[row, col].Value = $"Data_{row}_{col}";
                }
            }

            // Définir le CellArea à effacer (lignes 0-2, colonnes 0-2)
            CellArea clearArea = new CellArea();
            clearArea.StartRow = 0;
            clearArea.EndRow = 2;
            clearArea.StartColumn = 0;
            clearArea.EndColumn = 2;

            try
            {
                // Effacer la plage spécifiée
                worksheet.Cells.ClearRange(clearArea);
                Console.WriteLine("Cleared cells in range: Rows 0-2, Columns 0-2");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearRange method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("CellsMethodClearRangeWithCellAreaDemo.xlsx");
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ClearRange(int, int, int, int) {#clearrange_1}

Efface le contenu et le formatage d'une plage.

```csharp
public void ClearRange(int startRow, int startColumn, int endRow, int endColumn)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Indice de ligne de départ. |
| startColumn | Int32 | Indice de colonne de départ. |
| endRow | Int32 | Indice de ligne de fin. |
| endColumn | Int32 | Indice de colonne de fin. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodClearRangeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Remplir avec des données de test
            cells[0, 0].PutValue(1);
            cells[0, 16383].PutValue(2);
            cells[1048575, 0].PutValue(3);
            cells[1048575, 16383].PutValue(4);

            // Effacer toute la plage de la feuille de calcul
            cells.ClearRange(0, 0, 1048575, 16383);

            // Enregistrez le classeur
            workbook.Save("ClearRangeDemo.xlsx");

            Console.WriteLine("ClearRange demo executed successfully.");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


