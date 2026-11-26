---
title: "Range.ColumnWidth"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Range. Establece o obtiene el ancho de columna de este rango"
type: docs
url: /es/net/aspose.cells/range/columnwidth/
---
## Range.ColumnWidth property

Establece u obtiene el ancho de columna de este rango

```csharp
public double ColumnWidth { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangePropertyColumnWidthDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accede a un rango (columnas B a D)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B:D");
            
            // Muestra el ancho de columna actual
            Console.WriteLine("Current ColumnWidth: " + range.ColumnWidth);

            // Establece un nuevo ancho de columna (en unidades de carácter)
            range.ColumnWidth = 15.0;

            // Llena celdas para demostrar el efecto
            worksheet.Cells["B1"].PutValue("This is column B");
            worksheet.Cells["C1"].PutValue("This is column C");
            worksheet.Cells["D1"].PutValue("This is column D");

            // Ajustar automáticamente las filas para mostrar el contenido
            worksheet.AutoFitRows();

            // Guarda el libro de trabajo
            workbook.Save("ColumnWidthDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


