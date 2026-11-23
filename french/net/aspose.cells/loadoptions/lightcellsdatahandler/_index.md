---
title: "LoadOptions.LightCellsDataHandler"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LoadOptions. Le gestionnaire de données pour le traitement des données de cellules lors de la lecture du fichier modèle"
type: docs
url: /fr/net/aspose.cells/loadoptions/lightcellsdatahandler/
---
## LoadOptions.LightCellsDataHandler property

Le gestionnaire de données pour le traitement des données des cellules lors de la lecture du fichier modèle.

```csharp
public LightCellsDataHandler LightCellsDataHandler { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyLightCellsDataHandlerDemo
    {
        public static void Run()
        {
            // Créer un LightCellsDataHandler personnalisé pour traiter les données de cellules
            var dataHandler = new CustomLightCellsDataHandler();
            
            // Créer des options de chargement et définir le gestionnaire de données
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.LightCellsDataHandler = dataHandler;

            // Charger le classeur avec le gestionnaire personnalisé
            using (Workbook workbook = new Workbook("sample.xlsx", loadOptions))
            {
                Console.WriteLine("Workbook processed successfully with LightCellsDataHandler");
            }
        }
    }

    public class CustomLightCellsDataHandler : LightCellsDataHandler
    {
        public bool StartSheet(Worksheet sheet)
        {
            Console.WriteLine($"Processing sheet: {sheet.Name}");
            return true; // Continue processing this sheet
        }

        public bool StartRow(int rowIndex)
        {
            Console.WriteLine($"  Starting row: {rowIndex}");
            return true; // Continue processing this row
        }

        public bool ProcessRow(Row row)
        {
            // Vous pouvez traiter les données de ligne ici si nécessaire
            return true;
        }

        public bool StartCell(int columnIndex)
        {
            Console.WriteLine($"    Starting cell at column: {columnIndex}");
            return true; // Continue processing this cell
        }

        public bool ProcessCell(Cell cell)
        {
            Console.WriteLine($"      Cell[{cell.Row},{cell.Column}]: {cell.Value}");
            return true;
        }
    }
}
```

### Voir aussi

* interface [LightCellsDataHandler](../../lightcellsdatahandler/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


