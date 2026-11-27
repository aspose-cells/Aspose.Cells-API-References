---
title: "TextBoxCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextBoxCollection-egenskap. Hämtar TextBox-elementet på det angivna indexet"
type: docs
url: /sv/net/aspose.cells.drawing/textboxcollection/item/
---
## TextBoxCollection indexer (1 of 2)

Hämtar elementet [`TextBox`](../../textbox/) vid det angivna indexet.

```csharp
public TextBox this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Det nollbaserade indexet för elementet. |

### Returvärde

Elementet på det angivna indexet.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till några textrutor i kalkylbladet
            int textBoxIndex1 = worksheet.TextBoxes.Add(10, 10, 100, 50);
            TextBox textBox1 = worksheet.TextBoxes[textBoxIndex1];
            textBox1.Text = "TextBox 1";
            
            int textBoxIndex2 = worksheet.TextBoxes.Add(10, 70, 100, 50);
            TextBox textBox2 = worksheet.TextBoxes[textBoxIndex2];
            textBox2.Text = "TextBox 2";

            // Kom åt textrutor med Item‑egenskapen
            TextBoxCollection textBoxCollection = worksheet.TextBoxes;
            int index = textBoxCollection.Count - 1;
            TextBox lastTextBox = textBoxCollection[index];

            // Skriv ut texten i den sista textrutan
            Console.WriteLine("Last TextBox Text: " + lastTextBox.Text);
        }
    }
}
```

### Se även

* class [TextBox](../../textbox/)
* class [TextBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## TextBoxCollection indexer (2 of 2)

Hämtar elementet [`TextBox`](../../textbox/) med namnet.

```csharp
public TextBox this[string name] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| namn | Namnet på textrutan. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till textrutor i kalkylbladet och hämta deras index
            int textBoxIndex1 = worksheet.TextBoxes.Add(10, 10, 100, 50);
            TextBox textBox1 = worksheet.TextBoxes[textBoxIndex1];
            textBox1.Name = "textbox 1";
            textBox1.Text = "First TextBox";

            int textBoxIndex2 = worksheet.TextBoxes.Add(10, 70, 100, 50);
            TextBox textBox2 = worksheet.TextBoxes[textBoxIndex2];
            textBox2.Name = "textbox 2";
            textBox2.Text = "Second TextBox";

            // Kom åt textrutan med Item‑egenskapen efter namn
            string txtboxName = "textbox 1";
            TextBox txb2 = worksheet.TextBoxes[txtboxName];
            if (txb2 != null)
            {
                Console.WriteLine("Found TextBox: " + txb2.Name);
                Console.WriteLine("TextBox Text: " + txb2.Text);
            }
        }
    }
}
```

### Se även

* class [TextBox](../../textbox/)
* class [TextBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


