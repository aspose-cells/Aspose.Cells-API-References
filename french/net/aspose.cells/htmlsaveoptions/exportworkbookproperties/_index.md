---
title: "HtmlSaveOptions.ExportWorkbookProperties"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Indique si l'exportation des propriétés du classeur est activée. La valeur par défaut est true. Si vous souhaitez importer le fichier html ou mht vers Excel, veuillez conserver la valeur par défaut."
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/exportworkbookproperties/
---
## HtmlSaveOptions.ExportWorkbookProperties property

Indiquant si l'exportation des propriétés du classeur est activée. La valeur par défaut est true. Si vous souhaitez importer le fichier html ou mht dans excel, veuillez conserver la valeur par défaut.

```csharp
public bool ExportWorkbookProperties { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportWorkbookPropertiesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter des données au classeur
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Définir les propriétés du classeur
            workbook.BuiltInDocumentProperties.Author = "Test Author";
            workbook.BuiltInDocumentProperties.Title = "Test Title";

            // Créer des options d'enregistrement HTML
            HtmlSaveOptions options = new HtmlSaveOptions();
            
            // Démontrer ExportWorkbookProperties en le définissant sur false
            options.ExportWorkbookProperties = false;
            
            // Enregistrez le classeur au format HTML
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML file saved with ExportWorkbookProperties set to false");
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


