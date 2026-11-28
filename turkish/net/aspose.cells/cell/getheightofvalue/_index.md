---
title: "Cell.GetHeightOfValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell yöntemi. Değerin yüksekliğini piksel biriminde alır"
type: docs
url: /tr/net/aspose.cells/cell/getheightofvalue/
---
## Cell.GetHeightOfValue method

Değerin yüksekliğini piksel biriminde al.

```csharp
public int GetHeightOfValue()
```

### Örnekler

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
            
            // Değeri ayarlayın ve yüksekliği ölçün
            worksheet.Cells["A1"].PutValue("Sample Text");
            double height = worksheet.Cells["A1"].GetHeightOfValue();
            
            Console.WriteLine("Height of value in A1: " + height);
            
            // Satır yüksekliğini ayarlayın ve tekrar ölçün
            worksheet.Cells.Rows[0].Height = 30;
            height = worksheet.Cells["A1"].GetHeightOfValue();
            
            Console.WriteLine("Height after row adjustment: " + height);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


