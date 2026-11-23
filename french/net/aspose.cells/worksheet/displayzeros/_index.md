---
title: "Worksheet.DisplayZeros"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Vrai si les valeurs zéro sont affichées"
type: docs
url: /fr/net/aspose.cells/worksheet/displayzeros/
---
## Worksheet.DisplayZeros property

Vrai si les valeurs zéro sont affichées.

```csharp
public bool DisplayZeros { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyDisplayZerosDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Démontrez DisplayZeros = true (par défaut)
            sheet.DisplayZeros = true;
            Cell cell1 = sheet.Cells["A1"];
            cell1.PutValue(0);
            Console.WriteLine("DisplayZeros=true: " + cell1.StringValue);

            // Démontrez DisplayZeros = false
            sheet.DisplayZeros = false;
            Cell cell2 = sheet.Cells["A2"];
            cell2.PutValue(0);
            Console.WriteLine("DisplayZeros=false: " + cell2.StringValue);

            // Affichez le formatage personnalisé avec DisplayZeros
            Style style = wb.CreateStyle();
            style.Custom = "0.00;\"Zero\";\"Negative\"";
            Cell cell3 = sheet.Cells["A3"];
            cell3.PutValue(0);
            cell3.SetStyle(style);
            Console.WriteLine("Custom format with DisplayZeros=true: " + cell3.StringValue);

            sheet.DisplayZeros = false;
            Cell cell4 = sheet.Cells["A4"];
            cell4.PutValue(0);
            cell4.SetStyle(style);
            Console.WriteLine("Custom format with DisplayZeros=false: " + cell4.StringValue);
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


