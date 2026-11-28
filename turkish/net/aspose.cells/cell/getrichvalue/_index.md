---
title: "Cell.GetRichValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell yöntemi. Hücrenin zengin değerini alır"
type: docs
url: /tr/net/aspose.cells/cell/getrichvalue/
---
## Cell.GetRichValue method

Hücrenin zengin değerini al.

```csharp
public CellRichValue GetRichValue()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetRichValueDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet ws = wb.Worksheets[0];
            
            // A1 hücresine zengin metin değeri ayarlayın
            ws.Cells["A1"].PutValue("This is rich text");
            
            // A1 hücresinden zengin değeri alın
            CellRichValue richValue = ws.Cells["A1"].GetRichValue();
            
            // Zengin metin değerini göster
            Console.WriteLine("Rich Text Value: " + ws.Cells["A1"].StringValue);
            
            // Çalışma kitabını kaydedin
            wb.Save("RichValueDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CellRichValue](../../cellrichvalue/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


