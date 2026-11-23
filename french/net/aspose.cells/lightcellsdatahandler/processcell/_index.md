---
title: "LightCellsDataHandler.ProcessCell"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode LightCellsDataHandler. Commence à traiter une cellule"
type: docs
url: /fr/net/aspose.cells/lightcellsdatahandler/processcell/
---
## LightCellsDataHandler.ProcessCell method

Commence à traiter une cellule.

```csharp
public bool ProcessCell(Cell cell)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cellule | Cellule | Objet Cell qui est actuellement traité |

### Valeur de retour

indique si cette cellule doit être conservée dans le modèle de cellules de la feuille actuelle. En général, cela doit être false afin que toutes les cellules ne soient pas conservées en mémoire après leur traitement, ce qui permet d'économiser de la mémoire. Pour certains besoins spécifiques, comme lorsqu'un utilisateur doit accéder à certaines cellules plus tard après le traitement complet du classeur, l'utilisateur peut faire en sorte que cette méthode renvoie true pour garder ces cellules spéciales dans le modèle Cells et y accéder ultérieurement via des API telles que Cells[row, column]. Cependant, conserver les données des cellules dans le modèle Cells nécessite plus de mémoire et si toutes les cellules sont conservées, la lecture du fichier modèle en mode LightCells deviendra identique à la lecture en mode normal.

### Remarques

Il sera appelé après la lecture des données d'une cellule.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LightCellsDataHandlerMethodProcessCellWithCellDemo
    {
        public static void Run()
        {
            try
            {
                // Créer un fichier de données temporaire
                File.WriteAllText("input.txt", "A,B,C\n10,20,30\n40,50,60");

                // Créer des options de chargement avec un gestionnaire de cellules légères personnalisé
                LoadOptions loadOptions = new LoadOptions(LoadFormat.Csv);
                var handler = new CustomLightCellsDataHandler();
                loadOptions.LightCellsDataHandler = handler;

                // Charger le classeur avec le gestionnaire personnalisé
                Workbook workbook = new Workbook("input.txt", loadOptions);

                // Enregistrer les résultats traités
                workbook.Save("output.xlsx");
                Console.WriteLine("ProcessCell executed successfully. Check output.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ProcessCell: {ex.Message}");
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
                return true; // Process all cells
            }

            public bool ProcessCell(Cell cell)
            {
                // Doubler les valeurs numériques et marquer les chaînes
                if (cell.IsNumericValue)
                {
                    cell.PutValue(cell.DoubleValue * 2);
                }
                else if (cell.Type == CellValueType.IsString)
                {
                    cell.PutValue($"TEXT: {cell.StringValue}");
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

* class [Cell](../../cell/)
* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


