---
title: "WorkbookSettings.EnableMacros"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Habilitar macros"
type: docs
url: /es/net/aspose.cells/workbooksettings/enablemacros/
---
## WorkbookSettings.EnableMacros property

Habilitar macros;

```csharp
public bool EnableMacros { get; set; }
```

### Observaciones

Ahora solo funciona al copiar una hoja de cálculo a otra hoja en un libro de trabajo.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyEnableMacrosDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook wb = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet sheet = wb.Worksheets[0];
            
            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("Macro Test");
            
            // Demostrar la propiedad EnableMacros
            Console.WriteLine("Initial EnableMacros value: " + wb.Settings.EnableMacros);
            
            // Desactivar macros
            wb.Settings.EnableMacros = false;
            Console.WriteLine("After disabling macros: " + wb.Settings.EnableMacros);
            
            // Activar macros
            wb.Settings.EnableMacros = true;
            Console.WriteLine("After enabling macros: " + wb.Settings.EnableMacros);
            
            // Guarda el libro de trabajo
            wb.Save("EnableMacrosDemo.xlsx");
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


