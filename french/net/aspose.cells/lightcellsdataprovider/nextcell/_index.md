---
title: "LightCellsDataProvider.NextCell"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode LightCellsDataProvider. Obtient la prochaine cellule à enregistrer"
type: docs
url: /fr/net/aspose.cells/lightcellsdataprovider/nextcell/
---
## LightCellsDataProvider.NextCell method

Obtient la prochaine cellule à enregistrer.

```csharp
public int NextCell()
```

### Valeur de retour

l’index de colonne de la prochaine cellule à enregistrer. -1 signifie que la fin des données de la ligne actuelle a été atteinte et qu’aucune autre cellule de la ligne actuelle ne sera enregistrée.

### Remarques

Elle sera appelée au début de l’enregistrement d’une cellule.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderMethodNextCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Clear();
            
            var provider = new DemoLightCellsDataProvider();
            XlsSaveOptions saveOptions = new XlsSaveOptions { LightCellsDataProvider = provider };

            try
            {
                workbook.Save("NextCellDemo.xlsx", saveOptions);
                Console.WriteLine("Workbook saved with LightCellsDataProvider implementation");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        private class DemoLightCellsDataProvider : LightCellsDataProvider
        {
            private int rowIndex = -1;
            private int cellIndex = -1;
            private readonly object[,] data = new object[2, 2]
            {
                { "Column1", "Column2" },
                { 100, 200 }
            };

            public bool StartSheet(int sheetIndex) => sheetIndex == 0;

            public int NextRow()
            {
                rowIndex++;
                cellIndex = -1;
                return rowIndex < 2 ? 1 : 0;
            }

            public void StartRow(Row row) { }

            public int NextCell()
            {
                cellIndex++;
                return cellIndex < 2 ? 1 : 0;
            }

            public void StartCell(Cell cell)
            {
                cell.PutValue(data[rowIndex, cellIndex]);
            }

            public bool IsGatherString() => false;
        }
    }
}
```

### Voir aussi

* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


