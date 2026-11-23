---
title: "MarkdownSaveOptions.LightCellsDataProvider"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MarkdownSaveOptions. Le fournisseur de données pour fournir les données des cellules lors de l'enregistrement du classeur en mode léger"
type: docs
url: /fr/net/aspose.cells/markdownsaveoptions/lightcellsdataprovider/
---
## MarkdownSaveOptions.LightCellsDataProvider property

Le fournisseur de données pour fournir les données des cellules lors de l'enregistrement du classeur en mode léger.

```csharp
public LightCellsDataProvider LightCellsDataProvider { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections.Generic;

    public class MarkdownSaveOptionsPropertyLightCellsDataProviderDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplir des données d'exemple
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = "Item " + (i + 1);
                worksheet.Cells[i, 1].Value = i + 1;
            }

            // Créer un LightCellsDataProvider personnalisé
            var dataProvider = new CustomLightCellsDataProvider();

            // Créer MarkdownSaveOptions
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            
            // Afficher la valeur actuelle (devrait être null initialement)
            Console.WriteLine("Current LightCellsDataProvider value: " + (saveOptions.LightCellsDataProvider == null ? "null" : "set"));

            // Définir le fournisseur de données personnalisé
            saveOptions.LightCellsDataProvider = dataProvider;

            // Enregistrer avec le fournisseur de données personnalisé
            workbook.Save("LightCellsDataProviderDemo.md", saveOptions);
        }
    }

    public class CustomLightCellsDataProvider : LightCellsDataProvider
    {
        private List<string> items = new List<string> { "Apple", "Banana", "Cherry", "Date", "Elderberry" };
        private List<double> values = new List<double> { 1.99, 0.99, 2.99, 3.49, 4.99 };
        private int currentRow = -1;

        public bool StartSheet(int sheetIndex)
        {
            // Traiter uniquement la première feuille
            return sheetIndex == 0;
        }

        public int NextRow()
        {
            currentRow++;
            return currentRow < items.Count ? currentRow : -1;
        }

        public void StartRow(Row row)
        {
            // Définir la hauteur de la ligne si nécessaire
            row.Height = 15;
        }

        public int NextCell()
        {
            if (currentRow == -1)
            {
                // Ligne d'en-tête
                return currentRow < 2 ? currentRow + 1 : -1;
            }
            else
            {
                return currentRow < 2 ? currentRow + 1 : -1;
            }
        }

        public void StartCell(Cell cell)
        {
            if (currentRow == -1)
            {
                // En-tête
                if (cell.Column == 0)
                    cell.Value = "Product";
                else if (cell.Column == 1)
                    cell.Value = "Price";
            }
            else
            {
                // Données
                if (cell.Column == 0)
                    cell.Value = items[currentRow];
                else if (cell.Column == 1)
                    cell.Value = values[currentRow];
            }
        }

        public bool IsGatherString()
        {
            return false;
        }
    }
}
```

### Voir aussi

* interface [LightCellsDataProvider](../../lightcellsdataprovider/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


