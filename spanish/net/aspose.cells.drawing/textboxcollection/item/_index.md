---
title: "TextBoxCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextBoxCollection. Obtiene el elemento TextBox en el índice especificado"
type: docs
url: /es/net/aspose.cells.drawing/textboxcollection/item/
---
## TextBoxCollection indexer (1 of 2)

Obtiene el elemento [`TextBox`](../../textbox/) en el índice especificado.

```csharp
public TextBox this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice basado en cero del elemento. |

### Valor de retorno

El elemento en el índice especificado.

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega algunos cuadros de texto a la hoja de cálculo
            int textBoxIndex1 = worksheet.TextBoxes.Add(10, 10, 100, 50);
            TextBox textBox1 = worksheet.TextBoxes[textBoxIndex1];
            textBox1.Text = "TextBox 1";
            
            int textBoxIndex2 = worksheet.TextBoxes.Add(10, 70, 100, 50);
            TextBox textBox2 = worksheet.TextBoxes[textBoxIndex2];
            textBox2.Text = "TextBox 2";

            // Accede a los cuadros de texto usando la propiedad Item
            TextBoxCollection textBoxCollection = worksheet.TextBoxes;
            int index = textBoxCollection.Count - 1;
            TextBox lastTextBox = textBoxCollection[index];

            // Muestra el texto del último cuadro de texto
            Console.WriteLine("Last TextBox Text: " + lastTextBox.Text);
        }
    }
}
```

### Ver también

* class [TextBox](../../textbox/)
* class [TextBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## TextBoxCollection indexer (2 of 2)

Obtiene el elemento [`TextBox`](../../textbox/) por su nombre.

```csharp
public TextBox this[string name] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| name | El nombre del cuadro de texto. |

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega cuadros de texto a la hoja de cálculo y obtén sus índices
            int textBoxIndex1 = worksheet.TextBoxes.Add(10, 10, 100, 50);
            TextBox textBox1 = worksheet.TextBoxes[textBoxIndex1];
            textBox1.Name = "textbox 1";
            textBox1.Text = "First TextBox";

            int textBoxIndex2 = worksheet.TextBoxes.Add(10, 70, 100, 50);
            TextBox textBox2 = worksheet.TextBoxes[textBoxIndex2];
            textBox2.Name = "textbox 2";
            textBox2.Text = "Second TextBox";

            // Accede al cuadro de texto usando la propiedad Item por nombre
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

### Ver también

* class [TextBox](../../textbox/)
* class [TextBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


