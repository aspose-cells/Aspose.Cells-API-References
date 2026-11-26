---
title: "Worksheet.StartAccessCache"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Worksheet. Inicia la sesión que usa cachés para acceder a los datos en esta hoja de cálculo"
type: docs
url: /es/net/aspose.cells/worksheet/startaccesscache/
---
## Worksheet.StartAccessCache method

Inicia la sesión que usa cachés para acceder a los datos en esta hoja de cálculo.

```csharp
public void StartAccessCache(AccessCacheOptions opts)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| opciones | AccessCacheOptions | opciones de acceso a datos |

### Observaciones

Después de terminar el acceso a los datos, [`CloseAccessCache`](../closeaccesscache/) debe invocarse con las mismas opciones para borrar todas las cachés y recuperar el modo de acceso normal.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodStartAccessCacheWithAccessCacheOptionsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Establecer estilo predeterminado
            Style style = wb.DefaultStyle;
            style.Font.Size = 10;
            wb.DefaultStyle = style;

            // Agregar formato condicional
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            FormatConditionCollection fcc = cfc[cfc.Add()];
            fcc.AddArea(CellArea.CreateCellArea(0, 0, 10, 10));
            fcc.AddCondition(FormatConditionType.DuplicateValues);
            FormatCondition fc = fcc[0];
            fc.Style.Font.Size = 16;

            // Poblar algunos datos
            Cells cells = sheet.Cells;
            for (int i = 0; i < 10; i++)
            {
                cells[0, i].PutValue("A");
                cells[i, 0].PutValue(i);
            }

            // Iniciar caché de acceso para un mejor rendimiento
            sheet.StartAccessCache(AccessCacheOptions.ConditionalFormatting);

            // Verificar estilos
            for (int i = 0; i < 10; i++)
            {
                Console.WriteLine($"Cell[0,{i}] Font Size: {cells[0, i].GetDisplayStyle().Font.Size}");
                Console.WriteLine($"Cell[{i},0] Font Size: {cells[i, 0].GetDisplayStyle().Font.Size}");
            }

            // Cerrar caché al finalizar
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


