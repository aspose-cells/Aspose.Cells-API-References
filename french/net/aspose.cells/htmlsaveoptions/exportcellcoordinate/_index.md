---
title: "HtmlSaveOptions.ExportCellCoordinate"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Indique si les coordonnées Excel des cellules non vides sont exportées lors de l'enregistrement du fichier au format HTML. La valeur par défaut est false. Si vous souhaitez importer le HTML généré dans Excel, veuillez conserver la valeur par défaut."
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/exportcellcoordinate/
---
## HtmlSaveOptions.ExportCellCoordinate property

Indique si l'exportation des coordonnées excel des cellules non vides lors de l'enregistrement du fichier en html est activée. La valeur par défaut est false. Si vous souhaitez importer le html généré dans excel, veuillez conserver la valeur par défaut.

```csharp
public bool ExportCellCoordinate { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportCellCoordinateDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            // Créez des options d'enregistrement HTML et activez ExportCellCoordinate
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportCellCoordinate = true;

            // Enregistrez le classeur au format HTML avec les coordonnées des cellules
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML with cell coordinates exported successfully.");
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


