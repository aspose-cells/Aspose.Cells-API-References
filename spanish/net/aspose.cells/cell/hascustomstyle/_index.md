---
title: "Cell.HasCustomStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cell. Indica si esta celda tiene configuraciones de estilo personalizado diferentes del estilo predeterminado heredado de la fila, columna o libro de trabajo correspondiente"
type: docs
url: /es/net/aspose.cells/cell/hascustomstyle/
---
## Cell.HasCustomStyle property

Indica si esta celda tiene configuraciones de estilo personalizadas (diferentes de la predeterminada heredada de la fila, columna o libro de trabajo correspondiente).

```csharp
public bool HasCustomStyle { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellPropertyHasCustomStyleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y acceder a la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Check HasCustomStyle");

            // Muestre el valor inicial de HasCustomState (hereda el estilo predeterminado)
            Console.WriteLine("Initial HasCustomStyle: " + cell.HasCustomStyle);

            // Cree un estilo personalizado y aplíquelo a la celda
            Style customStyle = workbook.CreateStyle();
            customStyle.Font.IsBold = true;
            cell.SetStyle(customStyle);

            // Verifique que HasCustomStyle sea verdadero después de la modificación del estilo
            Console.WriteLine("After applying custom style - HasCustomStyle: " + cell.HasCustomStyle);

            // Guarde el libro de trabajo con el estilo personalizado aplicado
            workbook.Save("CellCustomStyleDemo.xlsx");

            // Restablezca el estilo de la celda al estilo predeterminado del libro de trabajo
            Style defaultStyle = workbook.DefaultStyle;
            cell.SetStyle(defaultStyle);

            // Verifique que HasCustomStyle sea falso después de volver al predeterminado
            Console.WriteLine("After resetting to default style - HasCustomStyle: " + cell.HasCustomStyle);
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


