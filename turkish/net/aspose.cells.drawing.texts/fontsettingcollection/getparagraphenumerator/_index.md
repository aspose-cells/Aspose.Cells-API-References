---
title: "FontSettingCollection.GetParagraphEnumerator"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FontSettingCollection yöntemi. Paragrafların enumerator'ını alır"
type: docs
url: /tr/net/aspose.cells.drawing.texts/fontsettingcollection/getparagraphenumerator/
---
## FontSettingCollection.GetParagraphEnumerator method

Paragrafların enumerator'ını alır.

```csharp
public IEnumerator GetParagraphEnumerator()
```

### Örnekler

```csharp
using System;
using System.Collections;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class FontSettingCollectionMethodGetParagraphEnumeratorDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets[0];

            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 300, 100);
            shape.Text = "First Paragraph\nSecond Paragraph\nThird Paragraph";

            int line = 0;
            for (IEnumerator ie = shape.TextBody.GetParagraphEnumerator(); ie.MoveNext(); )
            {
                TextParagraph paragraph = (TextParagraph)ie.Current;
                switch (line)
                {
                    case 0:
                        paragraph.AlignmentType = TextAlignmentType.Center;
                        break;
                    case 1:
                        paragraph.AlignmentType = TextAlignmentType.Left;
                        break;
                    case 2:
                        paragraph.AlignmentType = TextAlignmentType.Right;
                        break;
                }
                line++;
            }

            wb.Save("ParagraphEnumeratorExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


