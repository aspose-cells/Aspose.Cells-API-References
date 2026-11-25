---
title: "FontSettingCollection.GetParagraphEnumerator"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FontSettingCollection. Ottiene l'enumeratore dei paragrafi"
type: docs
url: /it/net/aspose.cells.drawing.texts/fontsettingcollection/getparagraphenumerator/
---
## FontSettingCollection.GetParagraphEnumerator method

Ottiene l'enumeratore dei paragrafi.

```csharp
public IEnumerator GetParagraphEnumerator()
```

### Esempi

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

### Vedi anche

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


