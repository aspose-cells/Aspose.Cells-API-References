---
title: "Enum TextDirectionType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.TextDirectionType enum. Bu paragraf için metin akış yönünü temsil eder"
type: docs
url: /tr/net/aspose.cells/textdirectiontype/
---
## TextDirectionType enumeration

Bu paragraf için metin akış yönünü temsil eder.

```csharp
public enum TextDirectionType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Context | `0` |  |
| LeftToRight | `1` |  |
| RightToLeft | `2` |  |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassTextDirectionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Sağdan sola metin yönünü ayarla
            Style style = cells["A1"].GetStyle();
            style.TextDirection = TextDirectionType.RightToLeft;
            cells["A1"].SetStyle(style);
            cells["A1"].PutValue("Right to Left Text");

            // Soldan sağa metin yönünü ayarla
            style = cells["A2"].GetStyle();
            style.TextDirection = TextDirectionType.LeftToRight;
            cells["A2"].SetStyle(style);
            cells["A2"].PutValue("Left to Right Text");

            // Bağlam metin yönünü ayarla
            style = cells["A3"].GetStyle();
            style.TextDirection = TextDirectionType.Context;
            cells["A3"].SetStyle(style);
            cells["A3"].PutValue("Context Text Direction");

            workbook.Save("TextDirectionTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


