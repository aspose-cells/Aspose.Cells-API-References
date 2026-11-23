---
title: "LowCodeHtmlSaveOptions.HtmlOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LowCodeHtmlSaveOptions. Les options générales pour l'enregistrement HTML"
type: docs
url: /fr/net/aspose.cells.lowcode/lowcodehtmlsaveoptions/htmloptions/
---
## LowCodeHtmlSaveOptions.HtmlOptions property

Les options générales pour l’enregistrement du HTML.

```csharp
public HtmlSaveOptions HtmlOptions { get; set; }
```

### Remarques

Lorsqu'une instance de [`HtmlSaveOptions`](../../../aspose.cells/htmlsaveoptions/) est spécifiée, le [`SaveFormat`](../saveformat/) sera écrasé (s'il avait été spécifié auparavant).

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeHtmlSaveOptionsPropertyHtmlOptionsDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.99);
            
            // Créer des options d'enregistrement HTML low-code
            LowCodeHtmlSaveOptions saveOptions = new LowCodeHtmlSaveOptions
            {
                SaveFormat = SaveFormat.Html,
                HtmlOptions = new HtmlSaveOptions()
            };

            // Afficher le paramètre d'exportation des lignes de grille actuel
            Console.WriteLine("Export gridlines initially: " + saveOptions.HtmlOptions.ExportGridLines);

            // Enregistrer avec les lignes de grille visibles
            workbook.Save("HtmlWithGridlines.html", saveOptions.HtmlOptions);

            // Modifier les options HTML pour masquer les lignes de grille
            saveOptions.HtmlOptions = new HtmlSaveOptions { ExportGridLines = false };
            Console.WriteLine("Export gridlines after modification: " + saveOptions.HtmlOptions.ExportGridLines);

            // Enregistrer sans lignes de grille
            workbook.Save("HtmlWithoutGridlines.html", saveOptions.HtmlOptions);

            Console.WriteLine("Demo executed successfully. Compare output files.");
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../../../aspose.cells/htmlsaveoptions/)
* class [LowCodeHtmlSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


