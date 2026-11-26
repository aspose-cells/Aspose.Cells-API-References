---
title: "Worksheet.Protection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Worksheet. Representa los distintos tipos de opciones de protección disponibles para una hoja de cálculo. Soporta opciones de protección avanzadas en ExcelXP y versiones posteriores."
type: docs
url: /es/net/aspose.cells/worksheet/protection/
---
## Worksheet.Protection property

Representa los diversos tipos de opciones de protección disponibles para una hoja de cálculo. Soporta opciones de protección avanzadas en ExcelXP y versiones posteriores.

```csharp
public Protection Protection { get; }
```

### Observaciones

Esta propiedad puede proteger la hoja de cálculo en todas las versiones de archivos Excel y soporta opciones de protección avanzadas en ExcelXP y versiones posteriores.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyProtectionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Acceder a las propiedades de protección
            Protection protection = sheet.Protection;
            
            // Establecer propiedades de protección
            protection.AllowEditingObject = false;
            protection.AllowEditingScenario = false;
            
            // Proteger la hoja de cálculo (usando el método Protect en lugar de establecer IsProtectedWithPassword directamente)
            sheet.Protect(ProtectionType.All, "password123", null);

            // Guarda el libro de trabajo
            workbook.Save("WorksheetProtectionDemo.xlsx");

            // Verificar la configuración de protección
            Console.WriteLine("AllowEditingObject: " + protection.AllowEditingObject);
            Console.WriteLine("AllowEditingScenario: " + protection.AllowEditingScenario);
        }
    }
}
```

### Ver también

* class [Protection](../../protection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


