---
title: "HtmlLoadOptions.AutoFitColsAndRows"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlLoadOptions. Indique s'il faut ajuster automatiquement les colonnes et les lignes. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/htmlloadoptions/autofitcolsandrows/
---
## HtmlLoadOptions.AutoFitColsAndRows property

Indique si les colonnes et lignes sont ajustées automatiquement. La valeur par défaut est false.

```csharp
public bool AutoFitColsAndRows { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyAutoFitColsAndRowsDemo
    {
        public static void Run()
        {
            // Créer des options de chargement HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
            
            // Activer l'ajustement automatique des colonnes et des lignes
            loadOptions.AutoFitColsAndRows = true;
            
            // Charger le fichier HTML avec les options spécifiées
            Workbook workbook = new Workbook("example.html", loadOptions);
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // L'ajustement automatique des colonnes et des lignes sera appliqué lors du chargement
            Console.WriteLine("Columns and rows have been auto-fitted during HTML import.");
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


