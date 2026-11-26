---
title: "CopyOptions.ExtendToAdjacentRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CopyOptions. Indica si se deben extender los rangos al copiar el rango a un rango adyacente"
type: docs
url: /es/net/aspose.cells/copyoptions/extendtoadjacentrange/
---
## CopyOptions.ExtendToAdjacentRange property

Indica si se extienden los rangos al copiar el rango a un rango adyacente.

```csharp
public bool ExtendToAdjacentRange { get; set; }
```

### Observaciones

Si es true, solo extiende el rango del hipervínculo, sin agregar un nuevo hipervínculo al copiar hipervínculos a filas adyacentes.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyExtendToAdjacentRangeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Agregue un hipervínculo a la celda A1
            ws.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // Crear opciones de copia y establecer ExtendToAdjacentRange a true
            CopyOptions copyOptions = new CopyOptions();
            copyOptions.ExtendToAdjacentRange = true;

            // Copiar la fila 0 a la fila 1 con las opciones de copia
            ws.Cells.CopyRows(ws.Cells, 0, 1, 1, copyOptions);

            // Verificar que el hipervínculo se extendió al rango adyacente
            Console.WriteLine("Hyperlink count after copy: " + ws.Hyperlinks.Count);
        }
    }
}
```

### Ver también

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


