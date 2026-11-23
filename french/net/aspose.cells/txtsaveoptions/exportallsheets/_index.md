---
title: "TxtSaveOptions.ExportAllSheets"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TxtSaveOptions. Indique si toutes les feuilles sont exportées vers le fichier texte. Si false, seule la feuille active est exportée, comme dans MS Excel"
type: docs
url: /fr/net/aspose.cells/txtsaveoptions/exportallsheets/
---
## TxtSaveOptions.ExportAllSheets property

Indique si toutes les feuilles sont exportées vers le fichier texte. Si false, seule la feuille active est exportée, comme dans MS Excel.

```csharp
public bool ExportAllSheets { get; set; }
```

### Remarques

La valeur par défaut est false.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyExportAllSheetsDemo
    {
        public static void Run()
        {
            // Créez un classeur avec deux feuilles
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Ajouter des données d'exemple aux deux feuilles
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[0].Cells["A2"].PutValue(1);
            workbook.Worksheets[1].Cells["A1"].PutValue("Sheet2 Data");
            workbook.Worksheets[1].Cells["A2"].PutValue(2);

            // Enregistrez avec ExportAllSheets=false (par défaut)
            TxtSaveOptions saveOptions = new TxtSaveOptions(SaveFormat.Csv);
            workbook.Save("output_single_sheet.csv", saveOptions);

            // Enregistrez avec ExportAllSheets=true
            saveOptions.ExportAllSheets = true;
            workbook.Save("output_all_sheets.csv", saveOptions);
        }
    }
}
```

### Voir aussi

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


