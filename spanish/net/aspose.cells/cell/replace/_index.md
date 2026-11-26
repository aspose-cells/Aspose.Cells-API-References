---
title: "Cell.Replace"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cell. Reemplazar texto de la celda con opciones"
type: docs
url: /es/net/aspose.cells/cell/replace/
---
## Cell.Replace method

Reemplaza el texto de la celda con opciones.

```csharp
public void Replace(string placeHolder, string newValue, ReplaceOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| placeHolder | String | Marcador de celda |
| newValue | String | Valor de cadena a reemplazar |
| opciones | ReplaceOptions | Las opciones de reemplazo |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodReplaceWithStringStringReplaceOptionsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Hello World");
            worksheet.Cells["A2"].PutValue("hello world");
            worksheet.Cells["A3"].PutValue("HELLO WORLD");
            worksheet.Cells["B1"].PutValue("Replaced");

            // Crear opciones de reemplazo
            ReplaceOptions options = new ReplaceOptions();
            options.CaseSensitive = false;
            options.MatchEntireCellContents = false;

            // Obtener configuración de fuente de la celda B1 para aplicar a los reemplazos
            options.FontSettings = worksheet.Cells["B1"].GetCharacters();

            // Reemplazar todas las variaciones de "hello" con "Hi" usando las opciones
            foreach (Cell cell in worksheet.Cells)
            {
                cell.Replace("Hello", "Hi", options);
            }

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [ReplaceOptions](../../replaceoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


