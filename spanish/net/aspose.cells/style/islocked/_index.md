---
title: "Style.IsLocked"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Style. Obtiene o establece un valor que indica si una celda puede modificarse o no"
type: docs
url: /es/net/aspose.cells/style/islocked/
---
## Style.IsLocked property

Obtiene o establece un valor que indica si una celda puede modificarse o no.

```csharp
public bool IsLocked { get; set; }
```

### Observaciones

Bloquear celdas no tiene efecto a menos que la hoja de cálculo esté protegida.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsLockedDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establecer la propiedad IsLocked para una celda
            Cell cell = cells["A1"];
            Style style = cell.GetStyle();
            style.IsLocked = true;
            cell.SetStyle(style);

            // Proteger la hoja de cálculo para aplicar el bloqueo
            worksheet.Protect(ProtectionType.All);

            // Verificar e imprimir el estado de IsLocked
            Console.WriteLine("Cell A1 IsLocked: " + cells["A1"].GetStyle().IsLocked);
            Console.WriteLine("Cell B1 IsLocked: " + cells["B1"].GetStyle().IsLocked);

            // Guarda el libro de trabajo
            workbook.Save("IsLockedDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


