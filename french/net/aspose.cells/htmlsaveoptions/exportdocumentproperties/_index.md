---
title: "HtmlSaveOptions.ExportDocumentProperties"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Indique si les propriétés du document sont exportées. La valeur par défaut est true. Si vous souhaitez importer le fichier html ou mht dans Excel, veuillez conserver la valeur par défaut"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/exportdocumentproperties/
---
## HtmlSaveOptions.ExportDocumentProperties property

Indiquant si l'exportation des propriétés du document est activée. La valeur par défaut est true. Si vous souhaitez importer le fichier html ou mht dans excel, veuillez conserver la valeur par défaut.

```csharp
public bool ExportDocumentProperties { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter quelques propriétés de document
            workbook.BuiltInDocumentProperties.Author = "Test Author";
            workbook.BuiltInDocumentProperties.Title = "Test Document";
            
            // Ajouter des données de cellules d'exemple
            worksheet.Cells["A1"].PutValue("Sample HTML Export");
            
            // Créer des options d'enregistrement HTML et définir ExportDocumentProperties sur false
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportDocumentProperties = false;
            
            // Enregistrez le classeur au format HTML
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML file saved with document properties export disabled.");
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


