---
title: "HtmlSaveOptions.WorksheetScalable"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Indique si le zoom avant ou arrière du html via le niveau de zoom de la feuille de calcul lors de l'enregistrement du fichier en html ; la valeur par défaut est false."
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/worksheetscalable/
---
## HtmlSaveOptions.WorksheetScalable property

Indique si le zoom avant ou arrière du HTML via le niveau de zoom de la feuille de calcul lors de l'enregistrement du fichier en HTML, la valeur par défaut est false.

```csharp
public bool WorksheetScalable { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyWorksheetScalableDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Définir les options d'enregistrement HTML avec la propriété WorksheetScalable.
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.WorksheetScalable = true;
            
            // Enregistrer le classeur avec les options HTML
            string outputPath = "output.html";
            workbook.Save(outputPath, options);
            
            // Vérifier que la sortie contient le style de mise à l'échelle.
            string htmlContent = File.ReadAllText(outputPath);
            Console.WriteLine("HTML contains scaling: " + htmlContent.Contains("transform: scale"));
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


