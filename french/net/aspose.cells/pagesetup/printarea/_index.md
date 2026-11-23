---
title: "PageSetup.PrintArea"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageSetup. Représente la plage à imprimer"
type: docs
url: /fr/net/aspose.cells/pagesetup/printarea/
---
## PageSetup.PrintArea property

Représente la plage à imprimer.

```csharp
public string PrintArea { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintAreaDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(2);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(3);
            
            // Définir la zone d'impression à A1:B3
            worksheet.PageSetup.PrintArea = "A1:B3";
            
            // Enregistrer avec uniquement la zone d'impression
            HtmlSaveOptions options = new HtmlSaveOptions
            {
                ExportPrintAreaOnly = true
            };
            
            workbook.Save("PrintAreaDemo.html", options);
            
            Console.WriteLine("Print area demo created successfully.");
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


