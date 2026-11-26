---
title: "ReplaceOptions.MatchEntireCellContents"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ReplaceOptions. Indica si se debe coincidir con todo el contenido de las celdas"
type: docs
url: /es/net/aspose.cells/replaceoptions/matchentirecellcontents/
---
## ReplaceOptions.MatchEntireCellContents property

Indica si se debe coincidir con el contenido completo de las celdas

```csharp
public bool MatchEntireCellContents { get; set; }
```

### Observaciones

El valor predeterminado es true.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReplaceOptionsPropertyMatchEntireCellContentsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer valores de celda de muestra
            worksheet.Cells["A1"].PutValue("apple");
            worksheet.Cells["A2"].PutValue("apple pie");
            worksheet.Cells["A3"].PutValue("an apple");
            worksheet.Cells["A4"].PutValue("apples");

            // Reemplazar con MatchEntireCellContents = true (solo coincidencia exacta)
            ReplaceOptions options1 = new ReplaceOptions();
            options1.MatchEntireCellContents = true;
            workbook.Replace("apple", "orange", options1);

            // Reemplazar con MatchEntireCellContents = false (coincidencia parcial)
            ReplaceOptions options2 = new ReplaceOptions();
            options2.MatchEntireCellContents = false;
            workbook.Replace("apple", "banana", options2);

            // Mostrar resultados
            Console.WriteLine("A1: " + worksheet.Cells["A1"].StringValue); // orange (exact match)
            Console.WriteLine("A2: " + worksheet.Cells["A2"].StringValue); // banana pie (partial match)
            Console.WriteLine("A3: " + worksheet.Cells["A3"].StringValue); // an banana (partial match)
            Console.WriteLine("A4: " + worksheet.Cells["A4"].StringValue); // bananas (partial match)
        }
    }
}
```

### Ver también

* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


