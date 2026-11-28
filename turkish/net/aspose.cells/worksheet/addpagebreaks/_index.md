---
title: "Worksheet.AddPageBreaks"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet yöntemi. Sayfa sonu ekler"
type: docs
url: /tr/net/aspose.cells/worksheet/addpagebreaks/
---
## Worksheet.AddPageBreaks method

Sayfa sonu ekler.

```csharp
public void AddPageBreaks(string cellName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellName | String |  |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAddPageBreaksWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Satır 1'de (B2) yatay sayfa sonu ekle
            worksheet.AddPageBreaks("B2");

            // Satır 9'da (B10) yatay sayfa sonu ekle
            worksheet.AddPageBreaks("B10");

            // İlk sayfa sonunun satır 1'de eklendiğini doğrula
            Console.WriteLine("First page break row: " + worksheet.HorizontalPageBreaks[0].Row);
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


