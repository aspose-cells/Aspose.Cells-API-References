---
title: "Range.EntireRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Range. Obtiene un objeto Range que representa la fila completa o filas que contienen el rango especificado"
type: docs
url: /es/net/aspose.cells/range/entirerow/
---
## Range.EntireRow property

Obtiene un objeto Range que representa la fila completa (o filas) que contiene el rango especificado.

```csharp
public Range EntireRow { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyEntireRowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Rellene algunos datos de ejemplo en la primera fila
            for (int col = 0; col < 5; col++)
            {
                sheet.Cells[0, col].PutValue($"Header {col + 1}");
            }

            // Obtenga la primera fila completa usando la propiedad EntireRow
            Aspose.Cells.Range entireRow = sheet.Cells.CreateRange("A1").EntireRow;

            // Copie la primera fila a la tercera fila
            Aspose.Cells.Range destination = sheet.Cells.CreateRange("A3").EntireRow;
            destination.Copy(entireRow);

            // Guarda el libro de trabajo
            workbook.Save("EntireRowDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


