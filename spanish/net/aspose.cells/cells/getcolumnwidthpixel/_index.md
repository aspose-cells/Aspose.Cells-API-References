---
title: "Cells.GetColumnWidthPixel"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Obtiene el ancho de la columna especificada en vista normal en unidades de píxel"
type: docs
url: /es/net/aspose.cells/cells/getcolumnwidthpixel/
---
## GetColumnWidthPixel(int) {#getcolumnwidthpixel}

Obtiene el ancho de la columna especificada en vista normal, en unidades de píxel.

```csharp
public int GetColumnWidthPixel(int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | Int32 | Índice de columna |

### Valor de retorno

Ancho de la columna en vista normal.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetColumnWidthPixelWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer el ancho de la columna en caracteres (se convertirá a píxeles)
            worksheet.Cells.SetColumnWidth(1, 25);
            
            // Obtener el ancho de la columna en píxeles
            int widthInPixels = worksheet.Cells.GetColumnWidthPixel(1);
            
            // Mostrar el resultado
            Console.WriteLine("Column width in pixels: " + widthInPixels);
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetColumnWidthPixel(int, bool) {#getcolumnwidthpixel_1}

Obtiene el ancho de la columna especificada en vista normal, en unidades de píxel.

```csharp
[Obsolete("Use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int GetColumnWidthPixel(int column, bool original)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | Int32 | Índice de columna |
| original | Booleano | Indica si se devuelve el ancho original incluso cuando la columna está oculta |

### Valor de retorno

Ancho de la columna en vista normal.

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método Cells.GetColumnWidth(int ,bool , CellsUnitType ). Este método será eliminado 12 meses después, a partir de abril de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetColumnWidthPixelWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y acceder a la primera hoja
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer el ancho estándar de la columna a 80 píxeles
            worksheet.Cells.StandardWidthPixels = 80;

            // Establecer el ancho específico para la columna 2 (tercera columna) a 120 píxeles
            worksheet.Cells.SetColumnWidthPixel(2, 120);

            try
            {
                // Obtener el ancho actual con modificaciones del usuario (original: false)
                int currentWidth = worksheet.Cells.GetColumnWidthPixel(2, false);
                Console.WriteLine($"Column 2 current width: {currentWidth} pixels");

                // Obtener el ancho original sin modificaciones (original: true)
                int originalWidth = worksheet.Cells.GetColumnWidthPixel(2, true);
                Console.WriteLine($"Column 2 original width: {originalWidth} pixels");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetColumnWidthPixel: {ex.Message}");
            }

            // Guardar el libro de trabajo para demostrar la persistencia del ancho de columna
            workbook.Save("ColumnWidthDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


