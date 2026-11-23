---
title: "JsonSaveOptions.SheetIndexes"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété JsonSaveOptions. Représente les index des feuilles exportées"
type: docs
url: /fr/net/aspose.cells/jsonsaveoptions/sheetindexes/
---
## JsonSaveOptions.SheetIndexes property

Représente les index des feuilles exportées.

```csharp
public int[] SheetIndexes { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class JsonSaveOptionsPropertySheetIndexesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur avec plusieurs feuilles
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Remplir quelques données dans chaque feuille
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Worksheet sheet = workbook.Worksheets[i];
                sheet.Cells["A1"].PutValue($"Data from Sheet {i + 1}");
            }

            // Créer une instance de JsonSaveOptions
            JsonSaveOptions options = new JsonSaveOptions();

            // Afficher les SheetIndexes actuels (null par défaut - exporte toutes les feuilles)
            Console.WriteLine("Current SheetIndexes: " + (options.SheetIndexes == null ? "Exporting all sheets" : string.Join(",", options.SheetIndexes)));

            // Définir pour n'exporter que la première et la troisième feuille (index 0 et 2)
            options.SheetIndexes = new int[] { 0, 2 };

            // Enregistrer en JSON avec les feuilles sélectionnées
            workbook.Save("JsonSaveOptionsPropertySheetIndexesDemo.json", options);

            // Vérifier en chargeant le JSON
            string jsonContent = System.IO.File.ReadAllText("JsonSaveOptionsPropertySheetIndexesDemo.json");
            Console.WriteLine("JSON Content:");
            Console.WriteLine(jsonContent);

            // Modifier pour n'exporter que la deuxième feuille (index 1)
            options.SheetIndexes = new int[] { 1 };
            workbook.Save("JsonSaveOptionsPropertySheetIndexesDemo_SingleSheet.json", options);

            // Vérifier l'exportation d'une seule feuille
            jsonContent = System.IO.File.ReadAllText("JsonSaveOptionsPropertySheetIndexesDemo_SingleSheet.json");
            Console.WriteLine("Single Sheet JSON Content:");
            Console.WriteLine(jsonContent);
        }
    }
}
```

### Voir aussi

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


