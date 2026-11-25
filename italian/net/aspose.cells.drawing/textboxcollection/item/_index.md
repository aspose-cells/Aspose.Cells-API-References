---
title: "TextBoxCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextBoxCollection. Ottiene l'elemento TextBox all'indice specificato"
type: docs
url: /it/net/aspose.cells.drawing/textboxcollection/item/
---
## TextBoxCollection indexer (1 of 2)

Ottiene l'elemento [`TextBox`](../../textbox/) all'indice specificato.

```csharp
public TextBox this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice a base zero dell'elemento. |

### Valore di ritorno

L'elemento all'indice specificato.

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcune caselle di testo al foglio di lavoro.
            int textBoxIndex1 = worksheet.TextBoxes.Add(10, 10, 100, 50);
            TextBox textBox1 = worksheet.TextBoxes[textBoxIndex1];
            textBox1.Text = "TextBox 1";
            
            int textBoxIndex2 = worksheet.TextBoxes.Add(10, 70, 100, 50);
            TextBox textBox2 = worksheet.TextBoxes[textBoxIndex2];
            textBox2.Text = "TextBox 2";

            // Accedi alle caselle di testo utilizzando la proprietà Item.
            TextBoxCollection textBoxCollection = worksheet.TextBoxes;
            int index = textBoxCollection.Count - 1;
            TextBox lastTextBox = textBoxCollection[index];

            // Restituisci il testo dell'ultima casella di testo.
            Console.WriteLine("Last TextBox Text: " + lastTextBox.Text);
        }
    }
}
```

### Vedi anche

* class [TextBox](../../textbox/)
* class [TextBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## TextBoxCollection indexer (2 of 2)

Ottiene l'elemento [`TextBox`](../../textbox/) per nome.

```csharp
public TextBox this[string name] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| name | Il nome della casella di testo. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi caselle di testo al foglio di lavoro e ottieni i loro indici.
            int textBoxIndex1 = worksheet.TextBoxes.Add(10, 10, 100, 50);
            TextBox textBox1 = worksheet.TextBoxes[textBoxIndex1];
            textBox1.Name = "textbox 1";
            textBox1.Text = "First TextBox";

            int textBoxIndex2 = worksheet.TextBoxes.Add(10, 70, 100, 50);
            TextBox textBox2 = worksheet.TextBoxes[textBoxIndex2];
            textBox2.Name = "textbox 2";
            textBox2.Text = "Second TextBox";

            // Accedi alla casella di testo usando la proprietà Item per nome.
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

### Vedi anche

* class [TextBox](../../textbox/)
* class [TextBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


