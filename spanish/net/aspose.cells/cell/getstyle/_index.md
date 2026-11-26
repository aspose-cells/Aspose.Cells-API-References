---
title: "Cell.GetStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cell. Obtiene el estilo de la celda"
type: docs
url: /es/net/aspose.cells/cell/getstyle/
---
## GetStyle() {#getstyle}

Obtiene el estilo de la celda.

```csharp
public Style GetStyle()
```

### Valor de retorno

Objeto Style.

### Observaciones

Para cambiar el estilo de la celda, por favor llame al método Cell.SetStyle() después de modificar el objeto style devuelto. Este método es igual que `GetStyle` con el valor true para el parámetro.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetStyleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establecer diferentes alineaciones verticales para las celdas
            cells["A1"].PutValue("Bottom Alignment");
            cells["A1"].GetStyle().VerticalAlignment = TextAlignmentType.Bottom;

            cells["A2"].PutValue("Center Alignment");
            cells["A2"].GetStyle().VerticalAlignment = TextAlignmentType.Center;

            cells["A3"].PutValue("Distributed Alignment");
            cells["A3"].GetStyle().VerticalAlignment = TextAlignmentType.Distributed;

            cells["A4"].PutValue("Justify Alignment");
            cells["A4"].GetStyle().VerticalAlignment = TextAlignmentType.Justify;

            cells["A5"].PutValue("Top Alignment");
            cells["A5"].GetStyle().VerticalAlignment = TextAlignmentType.Top;

            // Demostrar el método GetStyle()
            Console.WriteLine("A1 Vertical Alignment: " + cells["A1"].GetStyle().VerticalAlignment);
            Console.WriteLine("A2 Vertical Alignment: " + cells["A2"].GetStyle().VerticalAlignment);
            Console.WriteLine("A3 Vertical Alignment: " + cells["A3"].GetStyle().VerticalAlignment);
            Console.WriteLine("A4 Vertical Alignment: " + cells["A4"].GetStyle().VerticalAlignment);
            Console.WriteLine("A5 Vertical Alignment: " + cells["A5"].GetStyle().VerticalAlignment);
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

## GetStyle(bool) {#getstyle_1}

Si checkBorders es verdadero, verifica si los bordes de otras celdas afectarán el estilo de esta celda.

```csharp
public Style GetStyle(bool checkBorders)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| checkBorders | Booleano | Comprobar los bordes de otras celdas |

### Valor de retorno

Objeto Style.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetStyleWithBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder a una celda y establecer algunos datos de ejemplo
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue(123.456);

            // Obtener el estilo de la celda sin heredar de la fila/columna (parámetro false)
            Style style = cell.GetStyle(false);
            
            // Modificar el estilo
            style.Custom = "0.000";
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.None;

            // Aplicar el estilo modificado a la celda
            cell.SetStyle(style);

            // Verificar los cambios de estilo
            Console.WriteLine("Number Format: " + cell.GetStyle(false).Custom);
            Console.WriteLine("Top Border Style: " + cell.GetStyle(false).Borders[BorderType.TopBorder].LineStyle);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


