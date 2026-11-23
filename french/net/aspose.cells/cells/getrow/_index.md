---
title: "Cells.GetRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Obtient l'élément Row à l'index de ligne de cellule spécifié"
type: docs
url: /fr/net/aspose.cells/cells/getrow/
---
## Cells.GetRow method

Obtient l'élément [`Row`](../../row/) à l'index de ligne de cellule spécifié.

```csharp
[Obsolete("Use Cells.CheckRow(int row) instead.")]
public Row GetRow(int row)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | Indice de ligne |

### Valeur de retour

Si l'objet ligne existe, renvoie l'objet Row, sinon renvoie null.

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode Cells.CheckRow(int row). Cette méthode sera supprimée 12 mois plus tard à compter de février 2024. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetRowWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez des cellules dans la ligne 5 pour vous assurer que la ligne existe
            worksheet.Cells["A5"].PutValue("Row 5 Data");
            worksheet.Cells["B5"].PutValue(12345);

            try
            {
                // Appelez la méthode GetRow avec le paramètre Int32
                Row resultRow = worksheet.Cells.GetRow(5);

                if (resultRow != null)
                {
                    // Démontrez la manipulation des lignes
                    resultRow.Height = 20;
                    Console.WriteLine($"Retrieved row 5 successfully. Current height: {resultRow.Height} points");
                    
                    // Comptez les cellules dans la ligne
                    int cellCount = 0;
                    foreach (Cell cell in resultRow)
                    {
                        cellCount++;
                    }
                    Console.WriteLine($"Row 5 contains {cellCount} cells");
                }
                else
                {
                    Console.WriteLine("Row 5 not found in worksheet");
                }
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Invalid row index: {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRow: {ex.Message}");
            }

            // Enregistrer le classeur modifié
            workbook.Save("CellsMethodGetRowWithInt32Demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Row](../../row/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


