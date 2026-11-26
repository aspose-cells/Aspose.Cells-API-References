---
title: "Workbook.CloseAccessCache"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Workbook. Cierra la sesión que usa cachés para acceder a datos"
type: docs
url: /es/net/aspose.cells/workbook/closeaccesscache/
---
## Workbook.CloseAccessCache method

Cierra la sesión que utiliza cachés para acceder a los datos.

```csharp
public void CloseAccessCache(AccessCacheOptions opts)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| opciones | AccessCacheOptions | opciones de acceso a datos |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCloseAccessCacheWithAccessCacheOptionsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Agregar datos de ejemplo y formato condicional
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue(i % 2 == 0 ? "Data" : "Other");
            }

            // Agregar formato condicional
            int ruleIdx = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[ruleIdx];
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Equal, "Data", null);
            Style style = workbook.CreateStyle();
            style.Font.Size = 16;
            fcc.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 9, EndColumn = 0 });
            fcc[0].Style = style;

            // Iniciar caché de acceso para formato condicional
            workbook.StartAccessCache(AccessCacheOptions.ConditionalFormatting);

            // Acceder a celdas con formato condicional en caché
            for (int i = 0; i < 10; i++)
            {
                Cell cell = cells[i, 0];
                Console.WriteLine($"Cell {cell.Name}: Value={cell.StringValue}, FontSize={cell.GetDisplayStyle().Font.Size}");
            }

            // Cerrar el caché de acceso
            workbook.CloseAccessCache(AccessCacheOptions.ConditionalFormatting);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* enum [AccessCacheOptions](../../accesscacheoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


