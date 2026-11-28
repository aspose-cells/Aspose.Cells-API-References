---
title: "CellsHelper.GetTextWidth"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellsHelper yöntemi. Metnin genişliğini puan biriminde al"
type: docs
url: /tr/net/aspose.cells/cellshelper/gettextwidth/
---
## CellsHelper.GetTextWidth method

Metnin genişliğini nokta biriminde al.

```csharp
public static double GetTextWidth(string text, Font font, double scaling)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| metin | String | Metin. |
| yazı tipi | Yazı Tipi | Metnin yazı tipi. |
| ölçekleme | Double | Metnin ölçeklemesi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodGetTextWidthWithStringFontDoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Font font = workbook.DefaultStyle.Font;
            double textWidth = CellsHelper.GetTextWidth("Sample Text", font, 1.0);
            Console.WriteLine("Text width: " + textWidth);
        }
    }
}
```

### Ayrıca Bakınız

* class [Font](../../font/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


