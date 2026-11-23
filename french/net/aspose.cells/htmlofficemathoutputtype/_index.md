---
title: "Enum HtmlOfficeMathOutputType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.HtmlOfficeMathOutputType enum. Représente la façon d'exporter OfficeMath en HTML"
type: docs
url: /fr/net/aspose.cells/htmlofficemathoutputtype/
---
## HtmlOfficeMathOutputType enumeration

Représente la façon d'exporter OfficeMath en HTML.

```csharp
public enum HtmlOfficeMathOutputType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Image | `0` | Convertit OfficeMath en HTML sous forme d'image spécifiée par la balise &lt;img&gt;. |
| MathML | `1` | Convertit OfficeMath en HTML en utilisant MathML. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class CellsClassHtmlOfficeMathOutputTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter OfficeMath à la cellule A1
            worksheet.Cells["A1"].PutValue("=SUM(1,2)");
            
            // Créer des options d'enregistrement HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Définir le type de sortie OfficeMath sur Image
            saveOptions.OfficeMathOutputMode = HtmlOfficeMathOutputType.Image;
            
            // Enregistrer avec le type de sortie Image
            workbook.Save("HtmlOfficeMathOutputType_Image.html", saveOptions);
            
            // Modifier le type de sortie en MathML
            saveOptions.OfficeMathOutputMode = HtmlOfficeMathOutputType.MathML;
            
            // Enregistrer avec le type de sortie MathML
            workbook.Save("HtmlOfficeMathOutputType_MathML.html", saveOptions);
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


