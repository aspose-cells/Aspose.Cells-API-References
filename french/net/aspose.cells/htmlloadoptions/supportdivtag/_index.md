---
title: "HtmlLoadOptions.SupportDivTag"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlLoadOptions. Indique si la mise en page de la balise div est prise en charge lorsque le fichier HTML la contient. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/htmlloadoptions/supportdivtag/
---
## HtmlLoadOptions.SupportDivTag property

Indique si la mise en page de la balise `<div>` est prise en charge lorsque le fichier html la contient. La valeur par défaut est false.

```csharp
public bool SupportDivTag { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertySupportDivTagDemo
    {
        public static void Run()
        {
            // Créer des options de chargement HTML avec SupportDivTag activé
            HtmlLoadOptions htmlLoadOptions = new HtmlLoadOptions(LoadFormat.Html);
            htmlLoadOptions.SupportDivTag = true;

            // Charger le fichier HTML avec des balises div
            Workbook workbook = new Workbook("input.html", htmlLoadOptions);

            // Accéder aux données de la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            // Exporter la valeur de la cellule et les informations de style
            Console.WriteLine("Cell A1 value: " + cell.StringValue);
            Console.WriteLine("Is bold: " + cell.GetStyle().Font.IsBold);

            // Enregistrer en tant que fichier Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


