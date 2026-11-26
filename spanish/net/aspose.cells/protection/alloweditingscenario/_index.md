---
title: "Protection.AllowEditingScenario"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Protection property. Representa si el usuario tiene permiso para editar escenarios en una hoja de cálculo protegida"
type: docs
url: /es/net/aspose.cells/protection/alloweditingscenario/
---
## Protection.AllowEditingScenario property

Representa si se permite al usuario editar escenarios en una hoja de cálculo protegida.

```csharp
public bool AllowEditingScenario { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowEditingScenarioDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(200);

            // Accede a la configuración de protección de la hoja de cálculo
            Protection protection = worksheet.Protection;

            // Configura las propiedades de protección con AllowEditingScenario habilitado
            protection.AllowEditingScenario = true;
            protection.AllowFormattingCell = true;  // Corrected property name
            protection.Password = "password123";

            // Proteger la hoja de cálculo
            worksheet.Protect(ProtectionType.All);

            // Guarda el libro de trabajo
            workbook.Save("ProtectionWithScenarioEditing.xlsx");

            Console.WriteLine("Worksheet protected with AllowEditingScenario enabled.");
        }
    }
}
```

### Ver también

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


