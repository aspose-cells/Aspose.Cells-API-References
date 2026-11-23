---
title: "SpreadsheetML2003SaveOptions.IsIndentedFormatting"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SpreadsheetML2003SaveOptions. Provoque l'indentation des éléments enfants"
type: docs
url: /fr/net/aspose.cells/spreadsheetml2003saveoptions/isindentedformatting/
---
## SpreadsheetML2003SaveOptions.IsIndentedFormatting property

Fait que les éléments enfants soient indentés.

```csharp
public bool IsIndentedFormatting { get; set; }
```

### Remarques

La valeur par défaut est true. Si la valeur est false, cela réduira la taille du fichier xml

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpreadsheetML2003SaveOptionsPropertyIsIndentedFormattingDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);

            // Configurez les options d'enregistrement avec un formatage indenté
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions
            {
                IsIndentedFormatting = true
            };

            // Enregistrez avec un formatage XML indenté
            workbook.Save("output_indented.xml", saveOptions);

            // Enregistrez sans formatage indenté pour la comparaison
            saveOptions.IsIndentedFormatting = false;
            workbook.Save("output_not_indented.xml", saveOptions);
        }
    }
}
```

### Voir aussi

* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


