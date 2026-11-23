---
title: "LightCellsDataHandler.StartCell"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode LightCellsDataHandler. Prépare le traitement d'une cellule"
type: docs
url: /fr/net/aspose.cells/lightcellsdatahandler/startcell/
---
## LightCellsDataHandler.StartCell method

Prépare le traitement d’une cellule.

```csharp
public bool StartCell(int columnIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | indice de colonne de la cellule à traiter |

### Valeur de retour

indique si cette cellule doit être traitée. false pour ignorer la cellule et vérifier la suivante jusqu'à atteindre la fin des données des cellules de la ligne actuelle

### Remarques

Il sera appelé lors de l'atteinte d'une cellule existante dans la ligne actuelle. La ligne actuelle est la ligne du dernier appel de [`ProcessRow`](../processrow/).

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LightCellsDataHandlerMethodStartCellWithInt32Demo
    {
        public static void Run()
        {
            try
            {
                // Créer un fichier d'entrée temporaire
                File.WriteAllText("input.csv", "Column1,Column2,Column3\n1,2,3\n4,5,6");

                // Créer des options de chargement avec un gestionnaire de cellules légères personnalisé
                LoadOptions loadOptions = new LoadOptions(LoadFormat.Csv);
                var handler = new CustomLightCellsDataHandler();
                loadOptions.LightCellsDataHandler = handler;

                // Charger le classeur avec le gestionnaire personnalisé
                Workbook workbook = new Workbook("input.csv", loadOptions);

                // Enregistrer le classeur traité
                workbook.Save("output.xlsx");
                Console.WriteLine("StartCell method executed successfully. Check output.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing StartCell method: {ex.Message}");
            }
        }

        private class CustomLightCellsDataHandler : LightCellsDataHandler
        {
            public bool StartSheet(Worksheet sheet)
            {
                return true; // Process all sheets
            }

            public bool StartRow(int rowIndex)
            {
                return true; // Process all rows
            }

            public bool StartCell(int columnIndex)
            {
                // Ne traiter que les cellules de l'indice de colonne 1 (deuxième colonne)
                return columnIndex == 1;
            }

            public bool ProcessCell(Cell cell)
            {
                // Doubler la valeur des cellules de la deuxième colonne
                if (cell.IsNumericValue)
                {
                    cell.PutValue(cell.DoubleValue * 2);
                }
                return true;
            }

            public bool ProcessRow(Row row)
            {
                return true; // Continue processing
            }
        }
    }
}
```

### Voir aussi

* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


