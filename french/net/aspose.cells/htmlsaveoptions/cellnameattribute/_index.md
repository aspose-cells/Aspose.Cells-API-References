---
title: "HtmlSaveOptions.CellNameAttribute"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Spécifie l'attribut qui indique le CellName à écrire. par ex. Si la valeur est id, alors pour la cellule A1 la sortie sera td idA1. La valeur par défaut est null"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/cellnameattribute/
---
## HtmlSaveOptions.CellNameAttribute property

Spécifie l'attribut qui indique le CellName à écrire. (par ex. Si la valeur est "id", alors pour la cellule "A1", la sortie sera :&lt;td id='A1'&gt;). La valeur par défaut est null.

```csharp
public string CellNameAttribute { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using System.Text.RegularExpressions;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyCellNameAttributeDemo
    {
        public static void Run()
        {
            // Créer un classeur d'exemple avec quelques données
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Data");
            worksheet.Cells["B2"].PutValue(123);

            // Définir les options d'enregistrement HTML avec CellNameAttribute
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.CellNameAttribute = "id";
            saveOptions.ExportImagesAsBase64 = true;
            saveOptions.ExportActiveWorksheetOnly = true;

            // Enregistrer dans un fichier HTML
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);

            // Vérifier que la sortie HTML contient les ID de cellules
            string htmlContent = File.ReadAllText(outputPath);
            Console.WriteLine("HTML contains A1 cell with ID: " + Regex.IsMatch(htmlContent, @"<td\s+id='A1'"));
            Console.WriteLine("HTML contains B2 cell with ID: " + Regex.IsMatch(htmlContent, @"<td\s+id='B2'"));
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


