---
title: "Cells.ConvertStringToNumericValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Çalışma sayfasındaki tüm metin verilerini mümkünse sayısal değere dönüştürür"
type: docs
url: /tr/net/aspose.cells/cells/convertstringtonumericvalue/
---
## Cells.ConvertStringToNumericValue method

Çalışma sayfasındaki tüm dize verilerini mümkünse sayısal değere dönüştürür.

```csharp
public void ConvertStringToNumericValue()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodConvertStringToNumericValueDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Sayısal değerlere dönüştürülebilecek dize değerlerini yerleştirin
            cells[0, 0].PutValue("1.23");
            cells[0, 1].PutValue("1.24");
            cells[0, 2].PutValue("1.23");
            cells[0, 3].PutValue("6/20/2021");
            cells[0, 4].PutValue("def"); // This will remain as string
            cells[0, 5].PutValue("6/20/2021");

            // Mümkün olduğunda dize değerlerini sayısala dönüştürün
            cells.ConvertStringToNumericValue();

            // Dönüştürülen değerleri gösterin
            Console.WriteLine("A1: " + cells[0, 0].DoubleValue);
            Console.WriteLine("B1: " + cells[0, 1].DoubleValue);
            Console.WriteLine("C1: " + cells[0, 2].DoubleValue);
            Console.WriteLine("D1: " + cells[0, 3].DoubleValue);
            Console.WriteLine("E1: " + cells[0, 4].StringValue); // Remains as string
            Console.WriteLine("F1: " + cells[0, 5].DoubleValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


