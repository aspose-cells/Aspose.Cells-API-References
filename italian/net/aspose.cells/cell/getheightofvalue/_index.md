---
title: "Cell.GetHeightOfValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cell. Ottiene l'altezza del valore in unità di pixel"
type: docs
url: /it/net/aspose.cells/cell/getheightofvalue/
---
## Cell.GetHeightOfValue method

Ottiene l'altezza del valore in unità di pixel.

```csharp
public int GetHeightOfValue()
```

### Esempi

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
            
            // Imposta il valore e misura l'altezza
            worksheet.Cells["A1"].PutValue("Sample Text");
            double height = worksheet.Cells["A1"].GetHeightOfValue();
            
            Console.WriteLine("Height of value in A1: " + height);
            
            // Regola l'altezza della riga e misura di nuovo
            worksheet.Cells.Rows[0].Height = 30;
            height = worksheet.Cells["A1"].GetHeightOfValue();
            
            Console.WriteLine("Height after row adjustment: " + height);
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


