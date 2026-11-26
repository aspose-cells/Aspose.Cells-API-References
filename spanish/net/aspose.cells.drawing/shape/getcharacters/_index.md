---
title: "Shape.GetCharacters"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Shape. Devuelve todos los objetos Characters que representan un rango de caracteres dentro del texto"
type: docs
url: /es/net/aspose.cells.drawing/shape/getcharacters/
---
## Shape.GetCharacters method

Devuelve todos los objetos Characters que representan un rango de caracteres dentro del texto.

```csharp
[Obsolete("Use Shape.GetRichFormattings() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList GetCharacters()
```

### Valor de retorno

Todos los objetos Characters

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, por favor use el método Shape.GetRichFormattings(). Este método será eliminado 12 meses después, a partir de noviembre de 2023. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using System.Collections;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetCharactersDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de cuadro de texto a la hoja de cálculo con todos los parámetros requeridos
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
            shape.Text = "Sample Text";

            // Obtener los caracteres de la forma
            ArrayList characters = shape.GetCharacters();

            // Mostrar información sobre cada carácter
            foreach (FontSetting charSetting in characters)
            {
                Console.WriteLine($"Font: {charSetting.Font.Name}, Size: {charSetting.Font.Size}");
            }
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


