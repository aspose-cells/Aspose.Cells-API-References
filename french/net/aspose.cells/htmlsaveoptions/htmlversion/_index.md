---
title: "HtmlSaveOptions.HtmlVersion"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Spécifie la version de la norme HTML qui doit être utilisée lors de l'enregistrement au format HTML. La valeur par défaut est HtmlVersion.Default"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/htmlversion/
---
## HtmlSaveOptions.HtmlVersion property

Spécifie la version de la norme HTML qui doit être utilisée lors de l’enregistrement au format HTML. La valeur par défaut est HtmlVersion.Default.

```csharp
public HtmlVersion HtmlVersion { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlSaveOptionsPropertyHtmlVersionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("HTML Version Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates HtmlVersion property");
            worksheet.Cells["B3"].PutValue(123.45);
            worksheet.Cells["C4"].PutValue("Sample Text");
            
            // Créer une instance de HtmlSaveOptions
            HtmlSaveOptions options = new HtmlSaveOptions();
            
            // Afficher la valeur actuelle de HtmlVersion
            Console.WriteLine("Current HtmlVersion: " + options.HtmlVersion);
            
            // Définir HtmlVersion sur HTML5
            options.HtmlVersion = HtmlVersion.Html5;
            Console.WriteLine("HtmlVersion changed to: " + options.HtmlVersion);
            
            // Enregistrer avec la version HTML5
            workbook.Save("HtmlVersion_Html5.html", options);
            
            // Passer à XHTML
            options.HtmlVersion = HtmlVersion.XHtml;
            Console.WriteLine("HtmlVersion changed to: " + options.HtmlVersion);
            
            // Enregistrer avec la version XHTML
            workbook.Save("HtmlVersion_XHtml.html", options);
            
            // Réinitialiser aux valeurs par défaut
            options.HtmlVersion = HtmlVersion.Default;
            Console.WriteLine("HtmlVersion reset to: " + options.HtmlVersion);
            
            // Enregistrer avec la version par défaut
            workbook.Save("HtmlVersion_Default.html", options);
        }
    }
}
```

### Voir aussi

* enum [HtmlVersion](../../htmlversion/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


