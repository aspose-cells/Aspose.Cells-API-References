---
title: "DeleteBlankOptions.EmptyFormulaValueAsBlank"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DeleteBlankOptions. Indica si una celda se considerará en blanco cuando es una fórmula y el resultado calculado es nulo o una cadena vacía. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/deleteblankoptions/emptyformulavalueasblank/
---
## DeleteBlankOptions.EmptyFormulaValueAsBlank property

Si una celda se considerará en blanco cuando es una fórmula y el resultado calculado es nulo o cadena vacía. El valor predeterminado es false.

```csharp
public bool EmptyFormulaValueAsBlank { get; set; }
```

### Observaciones

En general, el usuario debe asegurarse de que las fórmulas se hayan calculado antes de la operación de eliminación con esta propiedad establecida en true. De lo contrario, todas las fórmulas recién creadas mediante APIs normales como [`Formula`](../../cell/formula/) se considerarán en blanco y pueden ser eliminadas porque antes del cálculo sus resultados calculados son todos nulos.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyEmptyFormulaValueAsBlankDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Rellene datos de ejemplo
            cells["A1"].PutValue("Header");
            cells["A2"].Formula = "=B2";  // Formula returning blank
            cells["A3"].PutValue("Data");
            cells["A4"].Formula = "=1+1"; // Formula with value
            
            // Eliminar filas en blanco sin considerar los blancos de fórmulas
            Console.WriteLine("Before deletion (normal): " + cells.MaxRow + " rows");
            cells.DeleteBlankRows();
            Console.WriteLine("After normal deletion: " + cells.MaxRow + " rows");

            // Restablecer datos
            cells.ClearContents(0, 0, cells.MaxRow + 1, cells.MaxColumn + 1);
            cells["A1"].PutValue("Header");
            cells["A2"].Formula = "=B2";
            cells["A3"].PutValue("Data");
            cells["A4"].Formula = "=1+1";

            // Eliminar filas en blanco tratando los blancos de fórmulas como vacíos
            Console.WriteLine("\nBefore deletion (with EmptyFormulaValueAsBlank): " + cells.MaxRow + " rows");
            cells.DeleteBlankRows(new DeleteBlankOptions() { EmptyFormulaValueAsBlank = true });
            Console.WriteLine("After deletion with EmptyFormulaValueAsBlank: " + cells.MaxRow + " rows");
        }
    }
}
```

### Ver también

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


