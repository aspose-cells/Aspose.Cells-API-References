---
title: "WorksheetCollection.GetNamedRangesAndTables"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método WorksheetCollection. Obtiene todos los rangos con nombre predefinidos en la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/worksheetcollection/getnamedrangesandtables/
---
## WorksheetCollection.GetNamedRangesAndTables method

Obtiene todos los rangos con nombre predefinidos en la hoja de cálculo.

```csharp
public Range[] GetNamedRangesAndTables()
```

### Valor de retorno

Una matriz de objetos Range.

Devuelve null si el rango con nombre no existe.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodGetNamedRangesAndTablesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear algunos rangos con nombre
            worksheet.Cells.CreateRange("A1:B2").Name = "TestRange1";
            worksheet.Cells.CreateRange("C3:D4").Name = "TestRange2";
            
            // Obtener todos los rangos con nombre y tablas
            Aspose.Cells.Range[] ranges = workbook.Worksheets.GetNamedRangesAndTables();
            
            // Mostrar información sobre los rangos
            Console.WriteLine("Found {0} named ranges:", ranges.Length);
            foreach (Aspose.Cells.Range range in ranges)
            {
                Console.WriteLine("Name: {0}, Address: {1}", range.Name, range.Address);
            }
        }
    }
}
```

### Ver también

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


