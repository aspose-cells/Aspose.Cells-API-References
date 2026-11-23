---
title: "LightCellsDataProvider.StartRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode LightCellsDataProvider. Commence à enregistrer les données d’une ligne"
type: docs
url: /fr/net/aspose.cells/lightcellsdataprovider/startrow/
---
## LightCellsDataProvider.StartRow method

Commence à enregistrer les données d'une ligne.

```csharp
public void StartRow(Row row)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| row | Row | Objet Ligne destiné à l’implémentation pour remplir les données. Son index de ligne est la valeur renvoyée par le dernier appel de [`NextRow`](../nextrow/). Si la ligne a été initialisée dans le modèle interne des cellules, l’objet Ligne existant sera utilisé. Sinon, un objet Ligne temporaire sera utilisé pour que l’implémentation remplisse les données. |

### Remarques

Il sera appelé au début de l'enregistrement d'une ligne et de ses données de cellules. Si la ligne actuelle possède des propriétés personnalisées telles que la hauteur, le style, ...etc., l'implémentation doit définir ces propriétés sur l'objet Row fourni ici.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderMethodStartRowWithRowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer un fournisseur de données personnalisé
            var saveOptions = new OoxmlSaveOptions
            {
                LightCellsDataProvider = new CustomLightCellsDataProvider()
            };

            try
            {
                // Traiter le classeur avec notre fournisseur de données personnalisé
                workbook.Save("StartRowDemo.xlsx", saveOptions);
                Console.WriteLine("Workbook processed successfully with StartRow implementation.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing StartRow method: {ex.Message}");
            }
        }

        private class CustomLightCellsDataProvider : LightCellsDataProvider
        {
            private int currentRow = -1;
            private readonly int totalRows = 5;

            public bool StartSheet(int sheetIndex)
            {
                return sheetIndex == 0;
            }

            public int NextRow()
            {
                currentRow++;
                return currentRow < totalRows ? currentRow : -1;
            }

            public void StartRow(Row row)
            {
                // Démontrer la méthode StartRow avec le paramètre Row
                row.Height = 25;
                row.IsHidden = (currentRow % 2 == 0);
                Console.WriteLine($"Processing row {row.Index}, Height: {row.Height}, Hidden: {row.IsHidden}");
            }

            public int NextCell()
            {
                return 0; // Process only first cell in each row
            }

            public void StartCell(Cell cell)
            {
                cell.PutValue($"Row {cell.Row + 1} Data");
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

* class [Row](../../row/)
* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


