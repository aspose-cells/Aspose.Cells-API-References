---
title: "Protection.AllowFormattingRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Protection. Representa si el formato de filas está permitido en una hoja de cálculo protegida"
type: docs
url: /es/net/aspose.cells/protection/allowformattingrow/
---
## Protection.AllowFormattingRow property

Representa si se permite el formato de filas en una hoja de cálculo protegida

```csharp
public bool AllowFormattingRow { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowFormattingRowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Habilitar la protección de la hoja de cálculo
            worksheet.Protect(ProtectionType.All);

            // Acceder a la configuración de protección
            Protection protection = worksheet.Protection;

            // Permitir formatear filas mientras se mantienen otras protecciones
            protection.AllowFormattingRow = true;

            // Guarda el libro de trabajo
            workbook.Save("Protection_AllowFormattingRow.xlsx");
        }
    }
}
```

### Ver también

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


