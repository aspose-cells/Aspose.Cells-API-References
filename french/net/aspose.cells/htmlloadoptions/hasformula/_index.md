---
title: "HtmlLoadOptions.HasFormula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlLoadOptions. Indique si le texte est une formule s'il commence par"
type: docs
url: /fr/net/aspose.cells/htmlloadoptions/hasformula/
---
## HtmlLoadOptions.HasFormula property

Indique si le texte est une formule lorsqu'il commence par "=".

```csharp
public bool HasFormula { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyHasFormulaDemo
    {
        public static void Run()
        {
            // Créer des options de chargement HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
            
            // Définissez HasFormula sur false pour traiter les chaînes de formule comme du texte brut
            loadOptions.HasFormula = false;
            
            // Créer un classeur avec le fichier HTML et les options de chargement
            Workbook workbook = new Workbook("example.html", loadOptions);
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Afficher certaines valeurs de cellules pour démontrer l'importation HTML
            Console.WriteLine("A1: " + cells["A1"].StringValue);
            Console.WriteLine("B1: " + cells["B1"].StringValue);
            
            // Enregistrer au format XLSX
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


