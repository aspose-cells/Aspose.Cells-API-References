---
title: "Style.ToJson"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style yöntemi. Style'ı JSON yapı verisine dönüştür"
type: docs
url: /tr/net/aspose.cells/style/tojson/
---
## Style.ToJson method

[`Style`](../)'ı JSON yapı verisine dönüştür.

```csharp
public string ToJson()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodToJsonDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // B4 hücresine bir stil oluştur ve uygula
            Style style = workbook.CreateStyle();
            style.BackgroundColor = System.Drawing.Color.Yellow;
            cells["B4"].SetStyle(style);

            // Stili JSON'a dönüştür
            string styleJson = style.ToJson();
            Console.WriteLine("Style JSON:");
            Console.WriteLine(styleJson);

            // B6 hücresine formülü ayarlayın
            cells["B6"].Formula = "=A1";

            // Hücreyi JSON'a dönüştür
            string cellJson = cells["B6"].ToJson();
            Console.WriteLine("\nCell JSON:");
            Console.WriteLine(cellJson);
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


