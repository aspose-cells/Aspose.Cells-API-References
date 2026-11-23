---
title: "LightCellsDataProvider.StartCell"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode LightCellsDataProvider. Commence à enregistrer les données d’une cellule"
type: docs
url: /fr/net/aspose.cells/lightcellsdataprovider/startcell/
---
## LightCellsDataProvider.StartCell method

Commence à enregistrer les données d'une cellule.

```csharp
public void StartCell(Cell cell)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cell | Cell | Objet Cellule destiné à l’implémentation pour remplir les données. Son index de colonne est la valeur renvoyée par le dernier appel de [`NextCell`](../nextcell/). Si la cellule a été initialisée dans le modèle interne des cellules, l’objet Cellule existant sera utilisé. Sinon, un objet Cellule temporaire sera utilisé pour que l’implémentation remplisse les données. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderMethodStartCellWithCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer une cellule à utiliser comme paramètre
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Data");
            
            // Créer un fournisseur de données personnalisé
            var saveOptions = new OoxmlSaveOptions
            {
                LightCellsDataProvider = new CustomLightCellsDataProvider()
            };

            try
            {
                workbook.Save("StartCellWithCellDemo.xlsx", saveOptions);
                Console.WriteLine("Workbook saved with StartCell implementation");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        private class CustomLightCellsDataProvider : LightCellsDataProvider
        {
            private int rowIndex = -1;
            private int cellIndex = -1;
            private readonly int totalRows = 5;
            private readonly int totalCells = 3;

            public bool StartSheet(int sheetIndex)
            {
                return sheetIndex == 0;
            }

            public int NextRow()
            {
                rowIndex++;
                cellIndex = -1;
                return rowIndex < totalRows ? rowIndex : -1;
            }

            public void StartRow(Row row)
            {
                row.Height = 15;
            }

            public int NextCell()
            {
                cellIndex++;
                return cellIndex < totalCells ? cellIndex : -1;
            }

            public void StartCell(Cell cell)
            {
                cell.PutValue($"Row {cell.Row + 1}, Col {cell.Column + 1}");
            }

            public bool IsGatherString()
            {
                return false;
            }
        }
    }
}
```

### Voir aussi

* class [Cell](../../cell/)
* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


