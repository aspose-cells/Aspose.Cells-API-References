---
title: "Range.ColumnCount"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Range. Obtient le nombre de colonnes dans la plage"
type: docs
url: /fr/net/aspose.cells/range/columncount/
---
## Range.ColumnCount property

Obtient le nombre de colonnes dans la plage.

```csharp
public int ColumnCount { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyColumnCountDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet sheet = workbook.Worksheets[0];
            
            // Créez des données d'exemple (5 colonnes x 3 lignes)
            for (int col = 0; col < 5; col++)
            {
                for (int row = 0; row < 3; row++)
                {
                    sheet.Cells[row, col].PutValue($"Data {row},{col}");
                }
            }
            
            // Créez une plage couvrant toutes les colonnes de données
            Aspose.Cells.Range dataRange = sheet.Cells.CreateRange(0, 0, 3, 5);
            
            // Démontrez l'utilisation de ColumnCount
            Console.WriteLine($"Range has {dataRange.ColumnCount} columns");
            
            // Ajustez automatiquement chaque colonne de la plage
            for (int i = 0; i < dataRange.ColumnCount; i++)
            {
                sheet.AutoFitColumn(dataRange.FirstColumn + i);
            }
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


