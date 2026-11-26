---
title: "Font.Equals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Font. Verifica si dos fuentes son iguales"
type: docs
url: /es/net/aspose.cells/font/equals/
---
## Font.Equals method

Comprueba si dos fuentes son iguales.

```csharp
public bool Equals(Font font)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fuente | Fuente | Objeto de fuente comparado. |

### Valor de retorno

Verdadero si es igual al objeto de fuente comparado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontMethodEqualsWithFontDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Cree dos objetos de fuente para comparar
            Font font1 = workbook.CreateStyle().Font;
            font1.Name = "Arial";
            font1.Size = 12;
            font1.IsBold = true;
            font1.Color = System.Drawing.Color.Black;

            Font font2 = workbook.CreateStyle().Font;
            font2.Name = "Arial";
            font2.Size = 12;
            font2.IsBold = true;
            font2.Color = System.Drawing.Color.Black;

            try
            {
                // Llame al método Equals para comparar las fuentes
                bool areEqual = font1.Equals(font2);

                // Mostrar el resultado
                Console.WriteLine($"The fonts are equal: {areEqual}");

                // Modifique una fuente para que sean diferentes
                font2.IsItalic = true;
                areEqual = font1.Equals(font2);
                Console.WriteLine($"After modification, the fonts are equal: {areEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("FontEqualsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


