---
title: "Cell.Value"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cell. Obtiene/establece el valor contenido en esta celda"
type: docs
url: /es/net/aspose.cells/cell/value/
---
## Cell.Value property

Obtiene/establece el valor contenido en esta celda.

```csharp
public object Value { get; set; }
```

### Observaciones

Tipo posible:

null,

Boolean,

DateTime,

Double,

Integer

String.

Para un valor int, puede devolverse como un objeto Integer o un objeto Double. Y no hay garantía de que el valor devuelto se mantenga siempre como el mismo tipo de objeto.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyValueDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establecer valores usando la propiedad Value
            cells[0, 0].Value = "Product ID";
            cells[0, 1].Value = "Product Name";
            
            // Demostrar valores null
            cells[0, 2].Value = null;
            cells[1, 0].Value = null;
            cells[1, 1].Value = null;
            cells[1, 2].Value = null;

            // Mostrar valores
            Console.WriteLine("Cell[0,0] Value: " + cells[0, 0].Value);
            Console.WriteLine("Cell[0,1] Value: " + cells[0, 1].Value);
            Console.WriteLine("Cell[0,2] Value: " + (cells[0, 2].Value == null ? "null" : cells[0, 2].Value));
            Console.WriteLine("Cell[1,0] Value: " + (cells[1, 0].Value == null ? "null" : cells[1, 0].Value));
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


