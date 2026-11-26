---
title: "Shape.FormatCharacters"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Shape. Formatea algunos caracteres con la configuración de fuente"
type: docs
url: /es/net/aspose.cells.drawing/shape/formatcharacters/
---
## Shape.FormatCharacters method

Formatea algunos caracteres con la configuración de fuente.

```csharp
public void FormatCharacters(int startIndex, int length, Font font, StyleFlag flag)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startIndex | Int32 | El índice de inicio. |
| longitud | Int32 | La longitud. |
| fuente | Fuente | La configuración de fuente. |
| bandera | StyleFlag | La bandera de la configuración de fuente. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodFormatCharactersWithInt32Int32FontStyleFlagDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar un cuadro de texto a la hoja de cálculo
            Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
            textBox.Text = "Sample Text Formatting";
            
            // Crear una fuente con las propiedades deseadas
            Aspose.Cells.Font font = textBox.Font;
            font.Name = "Arial";
            font.Size = 12;
            font.IsBold = true;
            
            // Crear una bandera de estilo para especificar qué propiedades aplicar
            StyleFlag flag = new StyleFlag();
            flag.FontName = true;
            flag.FontSize = true;
            flag.FontBold = true;
            
            // Aplicar formato a caracteres específicos
            textBox.FormatCharacters(0, 6, font, flag);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Font](../../../aspose.cells/font/)
* class [StyleFlag](../../../aspose.cells/styleflag/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


