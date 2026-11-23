---
title: "SheetSet.Active"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SheetSet. Obtient un ensemble contenant la feuille active du classeur"
type: docs
url: /fr/net/aspose.cells.rendering/sheetset/active/
---
## SheetSet.Active property

Obtient un ensemble avec la feuille active du classeur.

```csharp
public static SheetSet Active { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetSetPropertyActiveDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur avec deux feuilles de calcul
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            
            // Définir la deuxième feuille de calcul comme active
            workbook.Worksheets.ActiveSheetIndex = 1;

            // Ajouter des données aux deux feuilles de calcul
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[1].Cells["A1"].PutValue("Active Sheet Data");

            // Créez les options d'enregistrement PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Enregistrer uniquement la feuille active
            pdfSaveOptions.SheetSet = SheetSet.Active;
            workbook.Save("ActiveSheetOnly.pdf", pdfSaveOptions);

            // Enregistrer toutes les feuilles pour comparaison
            pdfSaveOptions.SheetSet = SheetSet.All;
            workbook.Save("AllSheets.pdf", pdfSaveOptions);
        }
    }
}
```

### Voir aussi

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


