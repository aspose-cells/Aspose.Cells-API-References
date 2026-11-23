---
title: "HtmlSaveOptions.ExportImagesAsBase64"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Spécifie si les images sont enregistrées au format Base64 dans HTML, MHTML ou EPUB."
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/exportimagesasbase64/
---
## HtmlSaveOptions.ExportImagesAsBase64 property

Spécifie si les images sont enregistrées au format Base64 vers HTML, MHTML ou EPUB.

```csharp
public bool ExportImagesAsBase64 { get; set; }
```

### Remarques

Lorsque cette propriété est définie sur true, les données d'image sont exportées directement dans les éléments img et aucun fichier séparé n'est créé.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportImagesAsBase64Demo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une image à la feuille de calcul
            worksheet.Pictures.Add(0, 0, "example.jpg");
            
            // Créer des options d'enregistrement HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Définir ExportImagesAsBase64 sur true pour intégrer les images sous forme de chaînes base64.
            saveOptions.ExportImagesAsBase64 = true;
            
            // Enregistrer le classeur au format HTML avec des images intégrées.
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML with embedded images saved successfully.");
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


