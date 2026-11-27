---
title: "TextBoxCollection.RemoveAt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextBoxCollection-metod. Tar bort en textruta från filen"
type: docs
url: /sv/net/aspose.cells.drawing/textboxcollection/removeat/
---
## TextBoxCollection.RemoveAt method

Ta bort en textruta från filen.

```csharp
public void RemoveAt(int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | Textrutans index. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till några textrutor i kalkylbladet
            for (int i = 0; i < 3; i++)
            {
                worksheet.TextBoxes.Add(10, 10 + (i * 30), 200, 50);
                worksheet.TextBoxes[i].Text = "TextBox " + (i + 1);
            }

            Console.WriteLine("Before removal - TextBox count: " + worksheet.TextBoxes.Count);

            // Ta bort den sista textrutan med RemoveAt och en Int32-parameter
            int lastIndex = worksheet.TextBoxes.Count - 1;
            worksheet.TextBoxes.RemoveAt(lastIndex);

            Console.WriteLine("After removal - TextBox count: " + worksheet.TextBoxes.Count);
        }
    }
}
```

### Se även

* class [TextBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


