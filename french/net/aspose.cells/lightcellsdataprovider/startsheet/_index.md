---
title: "LightCellsDataProvider.StartSheet"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode LightCellsDataProvider. Commence à enregistrer une feuille de calcul"
type: docs
url: /fr/net/aspose.cells/lightcellsdataprovider/startsheet/
---
## LightCellsDataProvider.StartSheet method

Commence à enregistrer une feuille de calcul.

```csharp
public bool StartSheet(int sheetIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sheetIndex | Int32 | indice de la feuille actuelle à enregistrer. |

### Valeur de retour

true si ce fournisseur doit fournir des données pour la feuille donnée ; false si la feuille donnée doit utiliser son modèle de données normal (Cells).

### Remarques

Il sera appelé au début de l'enregistrement d'une feuille de calcul lors de l'enregistrement d'un classeur. Si le fournisseur doit se référer à

```csharp
sheetIndex
```

plus tard dans la méthode startRow(Row) ou startCell(Cell), c'est-à-dire, si le processus doit savoir quelle feuille de calcul est en cours de traitement, l'implémentation doit conserver le

```csharp
sheetIndex
```

valeur ici.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderMethodStartSheetWithInt32Demo
    {
        public static void Run()
        {
            try
            {
                Workbook workbook = new Workbook();
                workbook.Worksheets.Clear(); // Start with clean worksheet
                
                // Créer un fournisseur de données personnalisé et enregistrer en mode light cells
                var saveOptions = new OoxmlSaveOptions
                {
                    LightCellsDataProvider = new CustomLightCellsDataProvider()
                };

                Console.WriteLine("Starting workbook save with LightCellsDataProvider...");
                workbook.Save("StartSheetDemoOutput.xlsx", saveOptions);
                Console.WriteLine("Workbook saved successfully. Check StartSheetDemoOutput.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing demo: {ex.Message}");
            }
        }

        private class CustomLightCellsDataProvider : LightCellsDataProvider
        {
            private bool sheetProcessed = false;

            // Appelé lors du démarrage du traitement d’une feuille de calcul
            public bool StartSheet(int sheetIndex)
            {
                Console.WriteLine($"Processing sheet index: {sheetIndex}");
                // Traiter uniquement la première feuille (index 0)
                if (sheetIndex == 0)
                {
                    sheetProcessed = true;
                    return true;
                }
                return false;
            }

            public int NextRow()
            {
                if (sheetProcessed)
                {
                    sheetProcessed = false;
                    return 0; // Process first row (index 0)
                }
                return -1; // Stop processing after first row
            }

            public void StartRow(Row row)
            {
                row.Height = 20;
            }

            public int NextCell()
            {
                return 0; // Process first cell (index 0)
            }

            public void StartCell(Cell cell)
            {
                cell.PutValue("Data from LightCellsDataProvider");
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

* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


