---
title: "Cells.EndCellInRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Obtient la dernière cellule de cette ligne"
type: docs
url: /fr/net/aspose.cells/cells/endcellinrow/
---
## EndCellInRow(int) {#endcellinrow}

Obtient la dernière cellule de cette ligne.

```csharp
public Cell EndCellInRow(int rowIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Index de ligne. |

### Valeur de retour

Objet Cell.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodEndCellInRowWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Remplir les données dans la ligne 5 (index base 0)
            worksheet.Cells[5, 2].PutValue("Data1");
            worksheet.Cells[5, 4].PutValue("Data2");
            worksheet.Cells[5, 6].PutValue("Data3");

            try
            {
                // Appelez EndCellInRow avec l'index de ligne 5
                Cell endCell = worksheet.Cells.EndCellInRow(5);
                
                if (endCell != null)
                {
                    Console.WriteLine($"Last cell in row 5: {endCell.Name}");
                    Console.WriteLine($"Cell value: {endCell.StringValue}");
                }
                else
                {
                    Console.WriteLine("No cells found in row 5");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing EndCellInRow: {ex.Message}");
            }

            // Enregistrez le classeur
            workbook.Save("CellsMethodEndCellInRowWithInt32Demo.xlsx");
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

## EndCellInRow(int, int, int, int) {#endcellinrow_1}

Obtient la dernière cellule avec l'indice de ligne maximal dans cette plage.

```csharp
public Cell EndCellInRow(int startRow, int endRow, int startColumn, int endColumn)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Indice de ligne de départ. |
| endRow | Int32 | Indice de ligne de fin. |
| startColumn | Int32 | Indice de colonne de départ. |
| endColumn | Int32 | Indice de colonne de fin. |

### Valeur de retour

Objet Cell.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodEndCellInRowWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplir la feuille de calcul avec quelques données
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Cell_{i}_{j}");
                }
            }

            // Obtenez la cellule de fin dans la ligne 3 entre les colonnes 1 et 4
            Cell endCell = worksheet.Cells.EndCellInRow(3, 1, 3, 4);

            // Affichez les indices de ligne et de colonne de la cellule de fin
            Console.WriteLine($"End cell in row 3 between columns 1-4 is at: Row {endCell.Row}, Column {endCell.Column}");
        }
    }
}
```

### Voir aussi

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


