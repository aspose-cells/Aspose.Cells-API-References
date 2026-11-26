---
title: "Cell.StringValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cell. Obtiene el valor de cadena contenido en la celda. Si el tipo de esta celda es cadena, entonces devuelve el propio valor de cadena. Para otros tipos de celda, se devolverá el valor de cadena formateado con el estilo especificado de esta celda. El valor de celda formateado es el mismo que se puede obtener de Excel al copiar una celda como texto, como copiar la celda a un editor de texto o exportar a CSV."
type: docs
url: /es/net/aspose.cells/cell/stringvalue/
---
## Cell.StringValue property

Obtiene el valor de cadena contenido en la celda. Si el tipo de esta celda es cadena, entonces devuelve el propio valor de cadena. Para otros tipos de celda, se devolverá el valor de cadena formateado (formateado con el estilo especificado de esta celda). El valor de celda formateado es el mismo que se puede obtener de Excel al copiar una celda como texto (como copiar la celda a un editor de texto o exportar a csv).

```csharp
public string StringValue { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyStringValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establecer algunos valores
            cells["A1"].PutValue("Hello");
            cells["A2"].PutValue(123);
            cells["A3"].PutValue(DateTime.Now);
            cells["A4"].Formula = "=A1&A2";

            // Calcular fórmulas
            workbook.CalculateFormula();

            // Demostrar la propiedad StringValue
            Console.WriteLine("A1 StringValue: " + cells["A1"].StringValue);
            Console.WriteLine("A2 StringValue: " + cells["A2"].StringValue);
            Console.WriteLine("A3 StringValue: " + cells["A3"].StringValue);
            Console.WriteLine("A4 StringValue: " + cells["A4"].StringValue);

            // Mostrar caso de valor de error
            Cell errorCell = cells["B1"];
            errorCell.Formula = "=1/0";
            workbook.CalculateFormula();
            Console.WriteLine("B1 (Error) StringValue: " + errorCell.StringValue);
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


