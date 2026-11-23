---
title: "DocxSaveOptions.AsNormalView"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DocxSaveOptions. Exportation du fichier Excel vers un docx fiel en vue normale. Si cette propriété est true, une Area sera générée et aucune échelle ne sera appliquée. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/docxsaveoptions/asnormalview/
---
## DocxSaveOptions.AsNormalView property

Exportation d'un fichier Excel vers un fichier docx en vue normale. Si cette propriété est vraie, une zone sera générée et aucune échelle ne sera appliquée. La valeur par défaut est false.

```csharp
public bool AsNormalView { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DocxSaveOptionsPropertyAsNormalViewDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul et ajouter des données d’exemple
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Normal View Demo";

            try
            {
                // Initialiser DocxSaveOptions
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // Afficher la valeur par défaut de la propriété AsNormalView
                Console.WriteLine("Default AsNormalView value: " + saveOptions.AsNormalView);

                // Définir AsNormalView sur true pour démontrer son utilisation
                saveOptions.AsNormalView = true;
                Console.WriteLine("AsNormalView set to: " + saveOptions.AsNormalView);

                // Enregistrer le classeur au format DOCX avec les options configurées
                workbook.Save("AsNormalViewDemo.docx", saveOptions);
                Console.WriteLine("Document saved successfully with AsNormalView option.");
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


