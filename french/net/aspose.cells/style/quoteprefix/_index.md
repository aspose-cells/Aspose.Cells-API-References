---
title: "Style.QuotePrefix"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Style. Indique si la valeur de la cellule commence par un guillemet simple"
type: docs
url: /fr/net/aspose.cells/style/quoteprefix/
---
## Style.QuotePrefix property

Indique si la valeur de la cellule commence par un guillemet simple.

```csharp
public bool QuotePrefix { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyQuotePrefixDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accédez à la cellule B10 et définissez sa valeur
            Cell cell = worksheet.Cells["B10"];
            cell.PutValue("'12345"); // Note the single quote prefix

            // Obtenez le style de la cellule et activez QuotePrefix
            Style style = cell.GetStyle();
            style.QuotePrefix = true;
            cell.SetStyle(style);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");

            // Vérifiez la propriété QuotePrefix
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Cell loadedCell = loadedWorkbook.Worksheets[0].Cells["B10"];
            Console.WriteLine("QuotePrefix is set: " + loadedCell.GetStyle().QuotePrefix);
        }
    }
}
```

### Voir aussi

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


