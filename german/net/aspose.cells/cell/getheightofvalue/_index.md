---
title: "Cell.GetHeightOfValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Methode. Gibt die Höhe des Wertes in Pixeln zurück"
type: docs
url: /de/net/aspose.cells/cell/getheightofvalue/
---
## Cell.GetHeightOfValue method

Liefert die Höhe des Werts in der Einheit Pixel.

```csharp
public int GetHeightOfValue()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetHeightOfValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Wert setzen und Höhe messen
            worksheet.Cells["A1"].PutValue("Sample Text");
            double height = worksheet.Cells["A1"].GetHeightOfValue();
            
            Console.WriteLine("Height of value in A1: " + height);
            
            // Zeilenhöhe anpassen und erneut messen
            worksheet.Cells.Rows[0].Height = 30;
            height = worksheet.Cells["A1"].GetHeightOfValue();
            
            Console.WriteLine("Height after row adjustment: " + height);
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


