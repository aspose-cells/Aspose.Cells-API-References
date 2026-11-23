---
title: "LoadOptions.IgnoreNotPrinted"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LoadOptions. Ignorer les données qui ne sont pas imprimées lors de l'impression directe du fichier"
type: docs
url: /fr/net/aspose.cells/loadoptions/ignorenotprinted/
---
## LoadOptions.IgnoreNotPrinted property

Ignore les données qui ne sont pas imprimées lors de l'impression directe du fichier

```csharp
public bool IgnoreNotPrinted { get; set; }
```

### Remarques

Uniquement pour le fichier xlsx.

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyIgnoreNotPrintedDemo
    {
        public static void Run()
        {
            // Créer des options de chargement HTML et définir IgnoreNotPrinted
            HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
            loadOptions.IgnoreNotPrinted = true;
            loadOptions.AutoFitColsAndRows = true;

            // Charger le fichier HTML avec les options spécifiées
            Workbook workbook = new Workbook("example.html", loadOptions);
            Worksheet worksheet = workbook.Worksheets[0];

            // Démontrer l'effet de IgnoreNotPrinted en vérifiant les styles de cellule
            Console.WriteLine("B3 Cell Color: " + worksheet.Cells["B3"].GetStyle().ForegroundColor);
            Console.WriteLine("B4 Cell Color: " + worksheet.Cells["B4"].GetStyle().ForegroundColor);
            Console.WriteLine("B5 Cell Color: " + worksheet.Cells["B5"].GetStyle().ForegroundColor);

            // Enregistrez le classeur
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


