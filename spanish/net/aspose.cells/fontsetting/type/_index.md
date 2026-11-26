---
title: "FontSetting.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FontSetting. Obtiene el tipo de nodo de texto"
type: docs
url: /es/net/aspose.cells/fontsetting/type/
---
## FontSetting.Type property

Obtiene el tipo de nodo de texto.

```csharp
public virtual TextNodeType Type { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;  // Added this using directive
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingPropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar texto a una celda
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // Obtener la configuración de fuente para los caracteres de la celda
            FontSetting fontSetting = new FontSetting(0, 6, workbook.Worksheets);

            // Mostrar el valor actual de Type
            Console.WriteLine("Current Type value: " + fontSetting.Type);

            // Demostrar cómo el Tipo afecta el procesamiento del texto
            if (fontSetting.Type == TextNodeType.TextRun)
            {
                Console.WriteLine("The text is a standard text run.");
            }
            else if (fontSetting.Type == TextNodeType.TextParagraph)
            {
                Console.WriteLine("The text is part of a paragraph.");
            }
            else if (fontSetting.Type == TextNodeType.Equation)
            {
                Console.WriteLine("The text represents an equation.");
            }

            // Aplicar formato diferente según el Tipo
            if (fontSetting.Type == TextNodeType.TextRun)
            {
                fontSetting.Font.Color = System.Drawing.Color.Red;
                fontSetting.SetWordArtStyle(PresetWordArtStyle.WordArtStyle1);
            }

            // Guardar el resultado
            workbook.Save("FontSettingTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [TextNodeType](../../../aspose.cells.drawing.texts/textnodetype/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


