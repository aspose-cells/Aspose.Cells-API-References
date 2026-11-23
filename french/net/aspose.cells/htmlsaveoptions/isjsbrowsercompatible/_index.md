---
title: "HtmlSaveOptions.IsJsBrowserCompatible"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Indique si JavaScript est compatible avec les navigateurs qui ne supportent pas JavaScript. La valeur par défaut est true"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/isjsbrowsercompatible/
---
## HtmlSaveOptions.IsJsBrowserCompatible property

Indique si le JavaScript est compatible avec les navigateurs qui ne supportent pas JavaScript. La valeur par défaut est true.

```csharp
public bool IsJsBrowserCompatible { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsJsBrowserCompatibleDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test JavaScript Compatibility");

            // Configurer les options d'enregistrement HTML avec IsJsBrowserCompatible défini sur true
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                IsJsBrowserCompatible = true,
                ExportFormula = true,
                PresentationPreference = true
            };

            // Enregistrer le classeur avec la compatibilité JavaScript
            workbook.Save("JsCompatibleOutput.html", saveOptions);

            Console.WriteLine("HTML file with JavaScript compatibility saved successfully.");
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


