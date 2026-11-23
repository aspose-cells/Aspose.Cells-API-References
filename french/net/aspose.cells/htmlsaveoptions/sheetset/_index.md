---
title: "HtmlSaveOptions.SheetSet"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Obtient ou définit les feuilles à rendre. La valeur par défaut est toutes les feuilles visibles du classeur Visible"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/sheetset/
---
## HtmlSaveOptions.SheetSet property

Obtient ou définit les feuilles à rendre. La valeur par défaut est toutes les feuilles visibles du classeur : [`Visible`](../../../aspose.cells.rendering/sheetset/visible/).

```csharp
public SheetSet SheetSet { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class HtmlSaveOptionsPropertySheetSetDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec plusieurs feuilles de calcul
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // Masquez une feuille à des fins de démonstration
            workbook.Worksheets[1].IsVisible = false;

            // Définissez des données d'exemple dans chaque feuille
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Worksheet sheet = workbook.Worksheets[i];
                sheet.Cells["A1"].PutValue($"Data from {sheet.Name}");
            }

            // Créer une instance de HtmlSaveOptions
            HtmlSaveOptions options = new HtmlSaveOptions();

            // Affichez la valeur actuelle de SheetSet (la valeur par défaut est null, ce qui signifie toutes les feuilles visibles)
            Console.WriteLine("Current SheetSet value: " + (options.SheetSet == null ? "All visible sheets" : "Custom set"));

            // Définissez SheetSet pour n'inclure que des feuilles spécifiques (par index)
            options.SheetSet = new SheetSet(new int[] { 0, 2 });

            // Enregistrez au format HTML - seules les feuilles spécifiées seront incluses
            workbook.Save("HtmlWithCustomSheetSet.html", options);

            // Modifiez SheetSet pour n'inclure que les feuilles visibles
            options.SheetSet = SheetSet.Visible;
            workbook.Save("HtmlWithVisibleSheets.html", options);

            // Modifiez SheetSet pour n'inclure que la feuille active
            workbook.Worksheets[2].IsSelected = true; // Activate the sheet by selecting it
            options.SheetSet = SheetSet.Active;
            workbook.Save("HtmlWithActiveSheet.html", options);
        }
    }
}
```

### Voir aussi

* class [SheetSet](../../../aspose.cells.rendering/sheetset/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


