---
title: "PptxSaveOptions.IgnoreHiddenRows"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PptxSaveOptions. Indique s'il faut ignorer les lignes masquées lors de la conversion d'Excel vers PowerPoint"
type: docs
url: /fr/net/aspose.cells/pptxsaveoptions/ignorehiddenrows/
---
## PptxSaveOptions.IgnoreHiddenRows property

Indique s'il faut ignorer les lignes masquées lors de la conversion d'Excel vers PowerPoint.

```csharp
public bool IgnoreHiddenRows { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PptxSaveOptionsPropertyIgnoreHiddenRowsDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple et masquer certaines lignes
            worksheet.Cells["A1"].PutValue("Visible Row 1");
            worksheet.Cells["A2"].PutValue("Hidden Row");
            worksheet.Cells["A3"].PutValue("Visible Row 2");
            
            // Masquer la ligne 2
            worksheet.Cells.Rows[1].IsHidden = true;

            // Définir les options d'enregistrement PPTX avec IgnoreHiddenRows
            PptxSaveOptions saveOptions = new PptxSaveOptions();
            saveOptions.IgnoreHiddenRows = true;
            
            // Enregistrer en PPTX
            workbook.Save("output.pptx", saveOptions);
            
            Console.WriteLine("PPTX saved with hidden rows ignored.");
        }
    }
}
```

### Voir aussi

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


