---
title: "Cell.GetDisplayStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cell. Obtiene el estilo de visualización de esta celda"
type: docs
url: /es/net/aspose.cells/cell/getdisplaystyle/
---
## GetDisplayStyle() {#getdisplaystyle}

Obtiene el estilo de visualización de esta celda.

```csharp
public Style GetDisplayStyle()
```

### Valor de retorno

estilo de visualización de esta celda

### Observaciones

Igual que al usar SideBorders para `GetDisplayStyle`. Es decir, este método comprobará y ajustará los bordes superior/inferior/izquierdo/derecho de esta celda según el estilo([`GetStyle`](../getstyle/)) de sus celdas adyacentes, pero no comprobará las celdas combinadas, y no comprobará el estilo de visualización de las celdas adyacentes.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellMethodGetDisplayStyleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer estilo para la celda A1
            Style style1 = workbook.CreateStyle();
            style1.ForegroundColor = Color.FromArgb(157, 195, 230);
            worksheet.Cells["A1"].SetStyle(style1);
            
            // Establecer estilo para la celda A23
            Style style2 = workbook.CreateStyle();
            style2.ForegroundColor = Color.Red;
            worksheet.Cells["A23"].SetStyle(style2);
            
            // Obtener y mostrar estilos
            Style displayStyle1 = worksheet.Cells["A1"].GetDisplayStyle();
            Console.WriteLine("A1 Foreground Color: " + displayStyle1.ForegroundColor);
            
            Style displayStyle2 = worksheet.Cells["A23"].GetDisplayStyle();
            Console.WriteLine("A23 Foreground Color: " + displayStyle2.ForegroundColor);
        }
    }
}
```

### Ver también

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetDisplayStyle(bool) {#getdisplaystyle_2}

Obtiene el estilo de visualización de esta celda.

```csharp
public Style GetDisplayStyle(bool includeMergedBorders)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| includeMergedBorders | Booleano | Indica si se están comprobando los bordes de celdas combinadas. |

### Valor de retorno

estilo de visualización de esta celda

### Observaciones

Si la bandera especificada es falsa, entonces es igual que `GetDisplayStyle`. De lo contrario, es igual que al usar SideBorders&#x7C;DynamicStyleBorders para `GetDisplayStyle`.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetDisplayStyleWithBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Acceder a la celda B2 y establecer algunas propiedades de estilo
            Cell cell = worksheet.Cells["B2"];
            Style cellStyle = cell.GetStyle();
            cellStyle.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            cell.SetStyle(cellStyle);
            
            // Obtener estilo de visualización con formato (parámetro true)
            Style displayStyle = cell.GetDisplayStyle(true);
            
            // Mostrar el estilo de línea del borde derecho
            Console.WriteLine("Right Border Line Style: " + displayStyle.Borders[BorderType.RightBorder].LineStyle);
        }
    }
}
```

### Ver también

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetDisplayStyle(BorderType) {#getdisplaystyle_1}

Obtiene el estilo de visualización de esta celda.

```csharp
public Style GetDisplayStyle(BorderType adjacentBorders)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| adjacentBorders | BorderType | Indica qué bordes deben ser comprobados y ajustados según los bordes de las celdas adyacentes. |

### Valor de retorno

estilo de visualización de esta celda

### Observaciones

Si esta celda también está afectada por otras configuraciones como formato condicional, objetos de lista, etc., entonces el estilo de visualización puede ser diferente de [`GetStyle`](../getstyle/). Para las banderas que ajustan los bordes según las celdas adyacentes, TopBorder/BottomBorder/LeftBorder/RightBorder indican si se deben comprobar y combinar los bordes inferior/superior/derecho/izquierdo de las celdas izquierda/derecha/superior/inferior adyacentes a esta. Por razones de rendimiento y compatibilidad, se utilizan algunos enumerados para denotar operaciones especiales: Horizontal/Vertical indican si se deben comprobar y combinar el borde inferior/derecho de las celdas combinadas con esta. Diagonal (es decir, tanto DiagonalUpBorder como DiagonalDownBorder están configurados) indica que se deben comprobar y combinar los bordes del estilo de visualización de las celdas adyacentes. Tenga en cuenta que comprobar los bordes/estilos de las celdas adyacentes, especialmente los estilos de visualización, es un proceso que consume tiempo. Si no es necesario obtener los bordes para el estilo devuelto, usar None para desactivar el proceso de celdas adyacentes proporcionará mejor rendimiento. Al obtener los bordes de las celdas adyacentes a partir de los estilos definidos solo en esas celdas (sin configurar Diagonal), el rendimiento también puede ser mejor porque comprobar el estilo de visualización de una celda también consume tiempo.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetDisplayStyleWithBorderTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Establecer datos de muestra
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue(i);
            }

            // Crear formato condicional
            FormatConditionCollection fcs = sheet.ConditionalFormattings[sheet.ConditionalFormattings.Add()];
            fcs.AddArea(CellArea.CreateCellArea(0, 0, 9, 0));
            fcs.AddCondition(FormatConditionType.ColorScale);

            // Obtener estilo de visualización con diferentes tipos de borde
            for (int i = 0; i < 10; i++)
            {
                Style styleWithBorder = cells[i, 0].GetDisplayStyle(BorderType.TopBorder);
                Style styleWithoutBorder = cells[i, 0].GetDisplayStyle(BorderType.None);

                Console.WriteLine($"Cell {i + 1}:");
                Console.WriteLine($"  Style with border - Foreground: {styleWithBorder.ForegroundArgbColor:X}");
                Console.WriteLine($"  Style without border - Foreground: {styleWithoutBorder.ForegroundArgbColor:X}");
            }
        }
    }
}
```

### Ver también

* class [Style](../../style/)
* enum [BorderType](../../bordertype/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


