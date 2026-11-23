---
title: "HtmlSaveOptions.ExportArea"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Obtient ou définit la zone de cellules (CellArea) à exporter de la feuille de calcul active actuelle. Si vous définissez cet attribut, la zone d’impression de la feuille active sera omise. Seule la zone spécifiée sera exportée lors de l’enregistrement du fichier au format HTML."
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/exportarea/
---
## HtmlSaveOptions.ExportArea property

Obtient ou définit la CellArea d'exportation de la feuille de calcul active actuelle. Si vous définissez cet attribut, la zone d'impression de la feuille active sera omise. Seule la zone spécifiée sera exportée lors de l'enregistrement du fichier en html.

```csharp
public CellArea ExportArea { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportAreaDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplir la feuille de calcul avec quelques données
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Cell {i},{j}");
                }
            }

            // Définir les options d’enregistrement HTML avec la zone d’exportation
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportArea = CellArea.CreateCellArea("B2", "D5");

            // Enregistrez le classeur avec la zone d'exportation spécifiée
            workbook.Save("output.html", options);
        }
    }
}
```

### Voir aussi

* struct [CellArea](../../cellarea/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


