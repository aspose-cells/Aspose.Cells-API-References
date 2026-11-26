---
title: "Cells.GetCellDisplayStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Obtiene el estilo de visualización de la celda dada"
type: docs
url: /es/net/aspose.cells/cells/getcelldisplaystyle/
---
## GetCellDisplayStyle(int, int) {#getcelldisplaystyle}

Obtiene el estilo de visualización de la celda dada.

```csharp
public Style GetCellDisplayStyle(int row, int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | índice de fila de la celda dada |
| columna | Int32 | columna de la celda dada |

### Valor de retorno

el estilo de visualización de la celda dada.

### Observaciones

Lo mismo con [`GetDisplayStyle`](../../cell/getdisplaystyle/), y lo mismo al usar SideBorders para `GetCellDisplayStyle`.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetCellDisplayStyleWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Prepara el estilo de celda para la demostración
            Cell cell = cells[0, 0];
            cell.PutValue("Style Demo");
            
            // Crea un estilo personalizado
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            
            // Aplica el estilo a la celda
            cell.SetStyle(style);

            try
            {
                // Llama a GetCellDisplayStyle con fila 0 y columna 0
                Style displayStyle = cells.GetCellDisplayStyle(0, 0);

                // Propiedades del estilo de visualización
                Console.WriteLine($"Bold: {displayStyle.Font.IsBold}");
                Console.WriteLine($"Background Color: {displayStyle.ForegroundColor}");

                // Aplica el estilo de visualización a otra celda para verificación visual
                cells[2, 2].SetStyle(displayStyle);
                cells[2, 2].PutValue("Style Copied");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellDisplayStyle method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("CellsMethodGetCellDisplayStyleWithInt32Int32Demo.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../../style/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetCellDisplayStyle(int, int, BorderType) {#getcelldisplaystyle_1}

Obtiene el estilo de visualización de la celda dada.

```csharp
public Style GetCellDisplayStyle(int row, int column, BorderType adjacentBorders)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | índice de fila de la celda dada |
| columna | Int32 | columna de la celda dada |
| adjacentBorders | BorderType | Indica qué bordes deben revisarse y ajustarse según los bordes de las celdas adyacentes. Por favor, consulte la descripción del mismo parámetro de [`GetDisplayStyle`](../../cell/getdisplaystyle/). |

### Valor de retorno

el estilo de visualización de la celda dada.

### Observaciones

Si la celda también está afectada por otras configuraciones como formato condicional, objetos de lista, etc., entonces el estilo de visualización puede ser diferente de [`GetCellStyle`](../getcellstyle/). Y debido a que esas configuraciones también pueden aplicarse a celdas vacías (no existentes), usar este método puede evitar la instanciación de esas celdas vacías, por lo que el rendimiento será mejor que obtener la instancia Cell de Cells y luego llamar a [`GetDisplayStyle`](../../cell/getdisplaystyle/).

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetCellDisplayStyleWithInt32Int32BorderTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder a la celda A1 y establecer un estilo de borde
            Cell cell = worksheet.Cells["A1"];
            Style style = cell.GetStyle();
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Red;
            cell.SetStyle(style);

            try
            {
                // Llamar a GetCellDisplayStyle con parámetros específicos (0,0 para A1, tipo TopBorder)
                Style displayStyle = worksheet.Cells.GetCellDisplayStyle(0, 0, BorderType.TopBorder);

                // Verificar si el estilo recuperado coincide con nuestro color de borde
                if (displayStyle.Borders[BorderType.TopBorder].Color == System.Drawing.Color.Red)
                {
                    Console.WriteLine("Top border display style retrieved successfully - Color: Red");
                }

                // Demostrar la aplicación del estilo modificando otra celda
                Cell targetCell = worksheet.Cells["B1"];
                targetCell.SetStyle(displayStyle);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellDisplayStyle method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("GetCellDisplayStyleWithBorderTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../../style/)
* enum [BorderType](../../bordertype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


