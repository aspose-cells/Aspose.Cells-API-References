---
title: "HtmlSaveOptions.WidthScalable"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Indique si la largeur de colonne doit être exportée en unité d’échelle vers le HTML. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/widthscalable/
---
## HtmlSaveOptions.WidthScalable property

Indique si la largeur des colonnes est exportée en unité d'échelle vers HTML. La valeur par défaut est false.

```csharp
public bool WidthScalable { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyWidthScalableDemo
    {
        public static void Run()
        {
            // Créer un classeur d'exemple avec des données de test
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test WidthScalable Property");
            worksheet.Cells["B1"].PutValue(123.45);
            
            // Définissez les options d’enregistrement HTML avec la propriété WidthScalable
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.WidthScalable = true; // Demonstrate setting to true
            
            // Enregistrez avec une largeur évolutive
            workbook.Save("output_scalable.html", options);
            
            // Enregistrez à nouveau avec une largeur fixe
            options.WidthScalable = false;
            workbook.Save("output_fixed.html", options);
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


