---
title: "HtmlSaveOptions.CellCssPrefix"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Obtient et définit le préfixe du nom CSS. La valeur par défaut est"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/cellcssprefix/
---
## HtmlSaveOptions.CellCssPrefix property

Obtient et définit le préfixe du nom css, la valeur par défaut est "".

```csharp
public string CellCssPrefix { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyCellCssPrefixDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            // Définir les options d'enregistrement HTML avec CellCssPrefix
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.CellCssPrefix = "custom-cell-";

            // Enregistrer le classeur avec les options HTML
            workbook.Save("output.html", saveOptions);

            Console.WriteLine("HTML file saved with custom cell CSS prefix.");
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


