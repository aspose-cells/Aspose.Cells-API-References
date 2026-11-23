---
title: "LightCellsDataProvider.IsGatherString"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode LightCellsDataProvider. Vérifie si la valeur de chaîne actuelle de la cellule doit être rassemblée dans un pool global"
type: docs
url: /fr/net/aspose.cells/lightcellsdataprovider/isgatherstring/
---
## LightCellsDataProvider.IsGatherString method

Vérifie si la valeur chaîne actuelle de la cellule doit être rassemblée dans un pool global.

```csharp
public bool IsGatherString()
```

### Valeur de retour

true si la valeur de chaîne doit être rassemblée dans un pool global pour le fichier résultant.

### Remarques

La collecte des valeurs de chaîne n’est avantageuse que lorsqu’il existe de nombreuses valeurs de chaîne dupliquées pour les cellules fournies par cette implémentation. Dans ce cas, la collecte des chaînes permet d’économiser beaucoup de mémoire et de générer un fichier résultant plus petit. En revanche, s’il y a de nombreuses valeurs de chaîne pour les cellules fournies par LightCellsDataProvider mais que peu d’entre elles sont identiques, la collecte des chaînes consommera davantage de mémoire et de temps et n’apportera aucun avantage au fichier résultant.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderMethodIsGatherStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Clear();
            
            var saveOptions = new OoxmlSaveOptions
            {
                LightCellsDataProvider = new CustomLightCellsDataProvider()
            };

            try
            {
                workbook.Save("IsGatherStringDemo.xlsx", saveOptions);
                Console.WriteLine("Workbook saved with IsGatherString implementation");
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
            private readonly object[,] data = new object[3, 2]
            {
                { "Product", "Price" },
                { "Laptop", 1200.50 },
                { "Phone", 899.99 }
            };

            public bool StartSheet(int sheetIndex)
            {
                return sheetIndex == 0;
            }

            public int NextRow()
            {
                rowIndex++;
                cellIndex = -1;
                return rowIndex < 3 ? rowIndex : -1;
            }

            public void StartRow(Row row)
            {
                row.Height = 15;
            }

            public int NextCell()
            {
                cellIndex++;
                return cellIndex < 2 ? cellIndex : -1;
            }

            public void StartCell(Cell cell)
            {
                cell.PutValue(data[rowIndex, cellIndex]);
            }

            public bool IsGatherString()
            {
                // Collecter les chaînes uniquement pour la ligne d’en-tête (rowIndex 0)
                return rowIndex == 0;
            }
        }
    }
}
```

### Voir aussi

* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


