---
title: "HtmlSaveOptions.CalculateFormula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Indique s'il faut calculer les formules avant d'enregistrer le fichier HTML"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/calculateformula/
---
## HtmlSaveOptions.CalculateFormula property

Indique s'il faut calculer les formules avant d'enregistrer le fichier html.

```csharp
public bool CalculateFormula { get; set; }
```

### Remarques

La valeur par défaut est false.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyCalculateFormulaDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données et des formules à la feuille de calcul
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");

            // Créer HtmlSaveOptions avec CalculateFormula défini sur true
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                CalculateFormula = true
            };

            // Enregistrer le classeur au format HTML - les formules seront calculées
            workbook.Save("HtmlWithCalculatedFormulas.html", saveOptions);

            Console.WriteLine("HTML file with calculated formulas created successfully.");
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


