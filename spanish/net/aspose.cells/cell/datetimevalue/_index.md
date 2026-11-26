---
title: "Cell.DateTimeValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cell. Obtiene el valor DateTime contenido en la celda"
type: docs
url: /es/net/aspose.cells/cell/datetimevalue/
---
## Cell.DateTimeValue property

Obtiene el valor DateTime contenido en la celda.

```csharp
public DateTime DateTimeValue { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyDateTimeValueDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establecer un valor DateTime en la celda A1
            DateTime testDate = new DateTime(2023, 12, 25);
            cells["A1"].PutValue(testDate);

            // Formatear la celda para mostrar la fecha
            Style style = cells["A1"].GetStyle();
            style.Custom = "yyyy-MM-dd";
            cells["A1"].SetStyle(style);

            // Recuperar y verificar el DateTimeValue
            DateTime retrievedDate = cells["A1"].DateTimeValue;
            Console.WriteLine("Original DateTime: " + testDate.ToString("yyyy-MM-dd"));
            Console.WriteLine("Retrieved DateTime: " + retrievedDate.ToString("yyyy-MM-dd"));

            // Establecer otro valor DateTime en la celda B1
            DateTime anotherDate = new DateTime(2024, 1, 1);
            cells["B1"].PutValue(anotherDate);

            // Mostrar el DateTimeValue de B1
            Console.WriteLine("B1 DateTime: " + cells["B1"].DateTimeValue.ToString("yyyy-MM-dd"));
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


