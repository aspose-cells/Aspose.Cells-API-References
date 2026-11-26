---
title: "Protection.AllowFormattingCell"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Protection property. Representa si el formato de celdas está permitido en una hoja de cálculo protegida"
type: docs
url: /es/net/aspose.cells/protection/allowformattingcell/
---
## Protection.AllowFormattingCell property

Representa si se permite el formato de celdas en una hoja de cálculo protegida.

```csharp
public bool AllowFormattingCell { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowFormattingCellDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Habilitar la protección de la hoja de cálculo
            Protection protection = worksheet.Protection;
            
            // Configura varias propiedades de protección usando una bandera
            int flag = 0x40; // Only AllowFormattingCell flag is set
            protection.AllowFormattingCell = (flag & 0x40) != 0;

            // Verifique la configuración
            Console.WriteLine("AllowFormattingCell is set to: " + protection.AllowFormattingCell);

            // Guarda el libro de trabajo
            workbook.Save("ProtectionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


