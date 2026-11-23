---
title: "LowCodeHtmlSaveOptions.SaveFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LowCodeHtmlSaveOptions. Obtient et définit le format de la feuille de calcul"
type: docs
url: /fr/net/aspose.cells.lowcode/lowcodehtmlsaveoptions/saveformat/
---
## LowCodeHtmlSaveOptions.SaveFormat property

Obtient et définit le format de la feuille de calcul.

```csharp
public override SaveFormat SaveFormat { get; set; }
```

### Remarques

Lors de la modification de cette propriété, le format d'enregistrement spécifié par [`HtmlOptions`](../htmloptions/) sera ignoré (s'il avait été spécifié auparavant).

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeHtmlSaveOptionsPropertySaveFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample HTML Export");

            LowCodeHtmlSaveOptions options = new LowCodeHtmlSaveOptions();
            Console.WriteLine("Current SaveFormat value: " + options.SaveFormat);

            options.SaveFormat = SaveFormat.Html;
            options.HtmlOptions = new HtmlSaveOptions();

            workbook.Save("LowCodeHtmlExport.html", options.HtmlOptions);
        }
    }
}
```

### Voir aussi

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [LowCodeHtmlSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


