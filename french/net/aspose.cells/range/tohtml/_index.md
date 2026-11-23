---
title: "Range.ToHtml"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Range. Convertir la plage en html"
type: docs
url: /fr/net/aspose.cells/range/tohtml/
---
## Range.ToHtml method

Convertir la plage en html .

```csharp
public byte[] ToHtml(HtmlSaveOptions saveOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| saveOptions | HtmlSaveOptions | Options pour convertir la plage en html. |

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodToHtmlWithHtmlSaveOptionsDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Remplir quelques données dans la plage A1:J25
            for (int i = 0; i < 25; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].Value = $"Cell {i+1},{j+1}";
                }
            }

            // Créer une plage avec le nom de type entièrement qualifié
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:J25");
            
            // Créer des options d'enregistrement HTML
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportImagesAsBase64 = true;
            
            // Convertir la plage en HTML
            byte[] htmlData = range.ToHtml(options);
            
            // Enregistrer le HTML dans un fichier
            File.WriteAllBytes("output.html", htmlData);
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../../htmlsaveoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


