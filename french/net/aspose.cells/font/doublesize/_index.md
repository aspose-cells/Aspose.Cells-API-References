---
title: "Font.DoubleSize"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Font. Obtient et définit la taille double de la police"
type: docs
url: /fr/net/aspose.cells/font/doublesize/
---
## Font.DoubleSize property

Obtient et définit la double taille de la police.

```csharp
public double DoubleSize { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyDoubleSizeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            Style style = cell.GetStyle();
            style.Font.DoubleSize = 10.5;
            cell.SetStyle(style);
            
            Console.WriteLine("Font DoubleSize set to: " + cell.GetStyle().Font.DoubleSize);
        }
    }
}
```

### Voir aussi

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


