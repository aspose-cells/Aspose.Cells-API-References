---
title: "Shape.Characters"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Shape. Devuelve un objeto Characters que representa un rango de caracteres dentro del texto"
type: docs
url: /es/net/aspose.cells.drawing/shape/characters/
---
## Shape.Characters method

Devuelve un objeto Characters que representa un rango de caracteres dentro del texto.

```csharp
public FontSetting Characters(int startIndex, int length)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startIndex | Int32 | El índice del inicio del carácter. |
| longitud | Int32 | El número de caracteres. |

### Valor de retorno

Objeto Characters.

### Observaciones

Este método solo funciona en una forma con título.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodCharactersWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega una forma con texto
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);
            shape.Text = "Sample Text";

            // Obtener caracteres desde el índice 0 con longitud 4
            FontSetting fontSetting = shape.Characters(0, 4);
            
            // Modificar la configuración de fuente
            fontSetting.Font.Color = System.Drawing.Color.Red;
            fontSetting.Font.Size = 14;
            fontSetting.Font.IsBold = true;

            // Guarda el libro de trabajo
            workbook.Save("ShapeCharactersDemo.xlsx");
        }
    }
}
```

### Ver también

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


