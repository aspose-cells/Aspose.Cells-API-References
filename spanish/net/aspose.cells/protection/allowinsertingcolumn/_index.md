---
title: "Protection.AllowInsertingColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Protection. Representa si la inserción de columnas está permitida en una hoja de cálculo protegida"
type: docs
url: /es/net/aspose.cells/protection/allowinsertingcolumn/
---
## Protection.AllowInsertingColumn property

Representa si se permite la inserción de columnas en una hoja de cálculo protegida

```csharp
public bool AllowInsertingColumn { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowInsertingColumnDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtener la configuración de protección
            Protection protection = worksheet.Protection;

            // Establecer AllowInsertingColumn a true
            protection.AllowInsertingColumn = true;

            // Verifique la configuración
            Console.WriteLine("AllowInsertingColumn is set to: " + protection.AllowInsertingColumn);

            // Proteger la hoja de cálculo con contraseña (usando el método Workbook.Protect)
            workbook.Protect(ProtectionType.All, "password123");
            protection.AllowInsertingColumn = true; // Explicitly set again to demonstrate

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


