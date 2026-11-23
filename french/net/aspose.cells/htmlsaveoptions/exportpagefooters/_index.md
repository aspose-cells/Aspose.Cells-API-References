---
title: "HtmlSaveOptions.ExportPageFooters"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Indique si l'exportation des en-têtes de page"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/exportpagefooters/
---
## HtmlSaveOptions.ExportPageFooters property

Indique si l'exportation des en-têtes de page est activée.

```csharp
public bool ExportPageFooters { get; set; }
```

### Remarques

Fonctionne uniquement lorsque [`SaveAsSingleFile`](../saveassinglefile/) est vrai.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportPageFootersDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Créer des options d'enregistrement HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Définir ExportPageFooters sur vrai pour inclure les pieds de page dans la sortie
            saveOptions.ExportPageFooters = true;
            
            // Définir d'autres options nécessaires
            saveOptions.ExportPageHeaders = true;
            
            // Enregistrer le classeur au format HTML
            workbook.Save("HtmlWithPageFooters.html", saveOptions);
            
            Console.WriteLine("HTML file with page footers exported successfully.");
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


