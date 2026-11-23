---
title: "DocxSaveOptions.EmbedXlsxAsChartDataSource"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DocxSaveOptions. Indique si l\\'intégration d\\'un fichier xlsx comme source de données du graphique"
type: docs
url: /fr/net/aspose.cells/docxsaveoptions/embedxlsxaschartdatasource/
---
## DocxSaveOptions.EmbedXlsxAsChartDataSource property

Indique s'il faut intégrer un fichier xlsx comme source de données du graphique.

```csharp
public bool EmbedXlsxAsChartDataSource { get; set; }
```

### Remarques

La valeur par défaut est true.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DocxSaveOptionsPropertyEmbedXlsxAsChartDataSourceDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul et ajouter des données d’exemple
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Chart Data";

            try
            {
                // Initialiser DocxSaveOptions
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // Afficher la valeur par défaut de la propriété EmbedXlsxAsChartDataSource
                Console.WriteLine("Default EmbedXlsxAsChartDataSource value: " + saveOptions.EmbedXlsxAsChartDataSource);

                // Définir EmbedXlsxAsChartDataSource sur true pour démontrer son utilisation
                saveOptions.EmbedXlsxAsChartDataSource = true;
                Console.WriteLine("EmbedXlsxAsChartDataSource set to: " + saveOptions.EmbedXlsxAsChartDataSource);

                // Enregistrer le classeur au format DOCX avec les options configurées
                workbook.Save("EmbedXlsxAsChartDataSourceDemo.docx", saveOptions);
                Console.WriteLine("Document saved successfully with EmbedXlsxAsChartDataSource option.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


