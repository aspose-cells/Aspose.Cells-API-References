---
title: "CellsHelper.CellNameToIndex"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CellsHelper. Obtient les index de ligne et de colonne de la cellule selon son nom"
type: docs
url: /fr/net/aspose.cells/cellshelper/cellnametoindex/
---
## CellsHelper.CellNameToIndex method

Obtient les indices de ligne et de colonne de la cellule selon son nom.

```csharp
public static void CellNameToIndex(string cellName, out int row, out int column)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cellName | String | Nom de la cellule. |
| ligne | Int32& | Index de ligne de sortie |
| column | Int32& | Index de colonne de sortie |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperMethodCellNameToIndexWithStringInt32Int32Demo
    {
        public static void Run()
        {
            // Initialisez les variables pour contenir les index de ligne et de colonne
            int rowIndex = -1;
            int columnIndex = -1;
            string cellName = "C5";

            try
            {
                // Appelez la méthode CellNameToIndex pour convertir le nom de cellule en indices de ligne et de colonne
                CellsHelper.CellNameToIndex(cellName, out rowIndex, out columnIndex);

                // Affichez les résultats
                Console.WriteLine($"Cell name: {cellName}");
                Console.WriteLine($"Row index: {rowIndex}");
                Console.WriteLine($"Column index: {columnIndex}");

                // Créez un classeur et démontrez l'utilisation des indices
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Accédez à la cellule en utilisant les indices obtenus
                Cell cell = worksheet.Cells[rowIndex, columnIndex];
                cell.PutValue("Test Value");

                // Enregistrez le classeur
                workbook.Save("CellNameToIndexDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing CellNameToIndex method: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


