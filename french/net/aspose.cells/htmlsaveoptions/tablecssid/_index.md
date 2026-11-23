---
title: "HtmlSaveOptions.TableCssId"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Obtient et définit le préfixe du nom CSS de type tel que trcoltd, etc. Ils sont contenus dans l'élément table qui possède l'attribut TableCssId spécifique. La valeur par défaut est"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/tablecssid/
---
## HtmlSaveOptions.TableCssId property

Obtient et définit le préfixe du nom CSS de type tel que tr, col, td, etc., ils sont contenus dans l'élément table qui possède l'attribut TableCssId spécifique. La valeur par défaut est "".

```csharp
public string TableCssId { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyTableCssIdDemo
    {
        public static void Run()
        {
            // Créer un classeur d'exemple avec des données de test
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Configurer les options d'enregistrement HTML avec TableCssId
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            saveOptions.TableCssId = "custom-table-style";
            
            // Enregistrer le classeur avec les options HTML
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML file saved with TableCssId: " + saveOptions.TableCssId);
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


