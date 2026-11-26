---
title: "Style.IsProtectionApplied"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Style. Indica si se debe aplicar el formato de protección"
type: docs
url: /es/net/aspose.cells/style/isprotectionapplied/
---
## Style.IsProtectionApplied property

Indica si se debe aplicar el formato de protección.

```csharp
public bool IsProtectionApplied { get; set; }
```

### Observaciones

Solo para estilo con nombre.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsProtectionAppliedDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Cree un objeto de estilo
            Style style = workbook.CreateStyle();
            
            // Establecer propiedades de protección
            style.IsLocked = true;
            style.IsFormulaHidden = true;
            style.IsProtectionApplied = true;
            
            // Aplicar el estilo a una celda
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            
            // Verificar la configuración de protección
            Console.WriteLine("IsProtectionApplied: " + style.IsProtectionApplied);
            Console.WriteLine("IsLocked: " + style.IsLocked);
            Console.WriteLine("IsFormulaHidden: " + style.IsFormulaHidden);
            
            // Modificar la configuración de protección
            style.IsProtectionApplied = false;
            Console.WriteLine("\nAfter changing IsProtectionApplied to false:");
            Console.WriteLine("IsProtectionApplied: " + style.IsProtectionApplied);
        }
    }
}
```

### Ver también

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


