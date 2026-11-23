---
title: "FindOptions.CaseSensitive"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FindOptions. Indique si la chaîne recherchée est sensible à la casse"
type: docs
url: /fr/net/aspose.cells/findoptions/casesensitive/
---
## FindOptions.CaseSensitive property

Indique si la chaîne recherchée est sensible à la casse.

```csharp
public bool CaseSensitive { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyCaseSensitiveDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir des données d'exemple
            worksheet.Cells["A1"].PutValue("ABC");
            worksheet.Cells["A2"].PutValue("abc");
            worksheet.Cells["A3"].PutValue("BcD");

            FindOptions options = new FindOptions();
            options.CaseSensitive = true;
            
            // Rechercher \"bc\" avec sensibilité à la casse
            Cell cell = worksheet.Cells.Find("bc", null, options);
            
            Console.WriteLine(cell == null ? "Not found (case sensitive)" : $"Found at: {cell.Name}");
            
            options.CaseSensitive = false;
            cell = worksheet.Cells.Find("bc", null, options);
            
            Console.WriteLine(cell == null ? "Not found" : $"Found at: {cell.Name}");
        }
    }
}
```

### Voir aussi

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


