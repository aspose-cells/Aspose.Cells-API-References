---
title: "LoadOptions.LoadFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LoadOptions. Obtient le format de chargement"
type: docs
url: /fr/net/aspose.cells/loadoptions/loadformat/
---
## LoadOptions.LoadFormat property

Obtient le format de chargement.

```csharp
public LoadFormat LoadFormat { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LoadOptionsPropertyLoadFormatDemo
    {
        public static void Run()
        {
            // Créer un fichier CSV d'exemple
            File.WriteAllText("sample.csv", "Name,Age\nJohn,30\nAlice,25");

            // Créer LoadOptions pour le format CSV et afficher la propriété
            LoadOptions csvOptions = new LoadOptions(LoadFormat.Csv);
            Console.WriteLine("CSV LoadFormat: " + csvOptions.LoadFormat);

            // Charger le CSV avec les options correctes
            Workbook csvWorkbook = new Workbook("sample.csv", csvOptions);
            Console.WriteLine("CSV loaded cells: " + csvWorkbook.Worksheets[0].Cells["B1"].Value);

            // Créer LoadOptions pour le format XLSX et afficher la propriété
            LoadOptions xlsxOptions = new LoadOptions(LoadFormat.Xlsx);
            Console.WriteLine("\nXLSX LoadFormat: " + xlsxOptions.LoadFormat);

            // Créer/enregistrer un fichier XLSX d'exemple
            Workbook newWorkbook = new Workbook();
            newWorkbook.Worksheets[0].Cells["A1"].PutValue("XLSX LoadFormat demo");
            newWorkbook.Save("sample.xlsx");

            // Charger le XLSX avec les options correctes
            Workbook xlsxWorkbook = new Workbook("sample.xlsx", xlsxOptions);
            Console.WriteLine("XLSX loaded cell: " + xlsxWorkbook.Worksheets[0].Cells["A1"].Value);

            // Nettoyer les fichiers temporaires
            File.Delete("sample.csv");
            File.Delete("sample.xlsx");
        }
    }
}
```

### Voir aussi

* enum [LoadFormat](../../loadformat/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


