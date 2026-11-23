---
title: "HtmlSaveOptions.ShowAllSheets"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Indique s'il faut afficher toutes les feuilles lors de l'enregistrement en un seul fichier html"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/showallsheets/
---
## HtmlSaveOptions.ShowAllSheets property

Indique s’il faut afficher toutes les feuilles lors de l’enregistrement en un seul fichier HTML.

```csharp
public bool ShowAllSheets { get; set; }
```

### Remarques

Fonctionne uniquement lorsque [`SaveAsSingleFile`](../saveassinglefile/) est vrai.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyShowAllSheetsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur avec plusieurs feuilles
            Workbook workbook = new Workbook();
            
            // Ajouter des données à la première feuille
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Name = "FirstSheet";
            sheet1.Cells["A1"].PutValue("Sheet 1 Content");

            // Ajouter une deuxième feuille
            Worksheet sheet2 = workbook.Worksheets.Add("SecondSheet");
            sheet2.Cells["B2"].PutValue("Sheet 2 Content");

            // Ajouter une troisième feuille
            Worksheet sheet3 = workbook.Worksheets.Add("ThirdSheet");
            sheet3.Cells["C3"].PutValue("Sheet 3 Content");

            // Créer des options d'enregistrement HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Définir la propriété ShowAllSheets sur true pour exporter toutes les feuilles
            saveOptions.ShowAllSheets = true;

            // Enregistrer le classeur avec toutes les feuilles visibles en HTML
            workbook.Save("ShowAllSheetsDemo.html", saveOptions);

            Console.WriteLine("HTML file with all sheets exported successfully.");
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


