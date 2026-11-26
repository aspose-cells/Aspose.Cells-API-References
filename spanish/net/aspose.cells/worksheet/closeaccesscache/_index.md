---
title: "Worksheet.CloseAccessCache"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Worksheet. Cierra la sesión que usa cachés para acceder a los datos en esta hoja de cálculo"
type: docs
url: /es/net/aspose.cells/worksheet/closeaccesscache/
---
## Worksheet.CloseAccessCache method

Cierra la sesión que usa cachés para acceder a los datos en esta hoja de cálculo.

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
    public class WorksheetMethodCloseAccessCacheWithAccessCacheOptionsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Rellenar celdas con datos de ejemplo
            for (int i = 0; i < 1000; i++)
            {
                cells[i, 0].PutValue(i % 10);
            }

            // Agregar formato condicional
            FormatConditionCollection fcs = sheet.ConditionalFormattings[sheet.ConditionalFormattings.Add()];
            fcs.AddArea(CellArea.CreateCellArea(0, 0, 999, 0));
            fcs.AddCondition(FormatConditionType.ColorScale);

            // Habilitar caché de acceso para formato condicional
            sheet.StartAccessCache(AccessCacheOptions.ConditionalFormatting);

            // Realizar operaciones con acceso en caché
            Random random = new Random();
            for (int i = 0; i < 100; i++)
            {
                int r = random.Next(0, 1000);
                var style = cells[r, 0].GetDisplayStyle();
                Console.WriteLine($"Cell ({r},0) style: {style.ForegroundArgbColor:X}");
            }

            // Cerrar el caché de acceso
            sheet.CloseAccessCache(AccessCacheOptions.ConditionalFormatting);
        }
    }
}
```

### Ver también

* enum [AccessCacheOptions](../../accesscacheoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


