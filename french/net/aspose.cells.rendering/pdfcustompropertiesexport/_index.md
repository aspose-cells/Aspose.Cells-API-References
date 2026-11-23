---
title: "Enum PdfCustomPropertiesExport"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Rendering.PdfCustomPropertiesExport enum. Spécifie la façon dont CustomDocumentPropertyCollection sont exportées vers le fichier PDF"
type: docs
url: /fr/net/aspose.cells.rendering/pdfcustompropertiesexport/
---
## PdfCustomPropertiesExport enumeration

Spécifie la façon dont [`CustomDocumentPropertyCollection`](../../aspose.cells.properties/customdocumentpropertycollection/) sont exportées vers le fichier PDF.

```csharp
public enum PdfCustomPropertiesExport
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Aucune propriété personnalisée n'est exportée. |
| Standard | `1` | Les propriétés personnalisées sont exportées en tant qu'entrées dans le dictionnaire Info. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PdfCustomPropertiesExportDemo
    {
        public static void PdfCustomPropertiesExportExample()
        {
            // Créez un classeur et ajoutez des données
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello Aspose");
            worksheet.Cells["A2"].PutValue("This is a sample document");

            // Définissez quelques propriétés personnalisées
            workbook.Worksheets.CustomDocumentProperties.Add("Author", "John Doe");
            workbook.Worksheets.CustomDocumentProperties.Add("Subject", "Sample PDF Export");

            // Créez les options d'enregistrement PDF
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Définissez l'option d'exportation des propriétés personnalisées
            saveOptions.CustomPropertiesExport = PdfCustomPropertiesExport.Standard;

            // Enregistrez le classeur au format PDF
            workbook.Save("PdfCustomPropertiesExportExample.pdf", saveOptions);

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


