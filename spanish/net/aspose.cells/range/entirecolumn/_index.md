---
title: "Range.EntireColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Range. Obtiene un objeto Range que representa la columna completa o columnas que contienen el rango especificado"
type: docs
url: /es/net/aspose.cells/range/entirecolumn/
---
## Range.EntireColumn property

Obtiene un objeto Range que representa la columna completa (o columnas) que contiene el rango especificado.

```csharp
public Range EntireColumn { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyEntireColumnDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear un rango que comienza en la celda C1 (fila 0, columna 2)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 2, 1, 1);
            
            // Obtener la columna completa que contiene el rango (columna C)
            Aspose.Cells.Range entireColumn = range.EntireColumn;
            
            // Aplicar formato a la columna completa
            Style style = entireColumn[0, 0].GetStyle();
            style.Custom = "##0%";
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.NumberFormat = true;
            entireColumn.ApplyStyle(style, styleFlag);
            
            // Guarda el libro de trabajo
            workbook.Save("EntireColumnDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


