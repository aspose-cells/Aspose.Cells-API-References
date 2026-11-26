---
title: "StyleFlag.Locked"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad StyleFlag. Se aplicará la configuración de bloqueo"
type: docs
url: /es/net/aspose.cells/styleflag/locked/
---
## StyleFlag.Locked property

Se aplicará la configuración de bloqueo.

```csharp
public bool Locked { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyLockedDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crear un estilo y establecer su propiedad locked
            Style style = workbook.CreateStyle();
            style.IsLocked = true;

            // Crear una bandera de estilo y habilitar la bandera locked
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Locked = true;

            // Aplicar el estilo a la celda A1
            Cell cell = cells["A1"];
            cell.SetStyle(style, styleFlag);

            // Verificar el estado locked
            Console.WriteLine("Cell A1 is locked: " + cell.GetStyle().IsLocked);

            // Proteger la hoja de cálculo para ver el efecto de bloqueo
            worksheet.Protect(ProtectionType.All);

            // Intentar modificar la celda locked (generará una excepción cuando la hoja de cálculo esté protegida)
            try
            {
                cell.PutValue("Test");
                Console.WriteLine("Cell modified successfully (worksheet not properly protected)");
            }
            catch
            {
                Console.WriteLine("Could not modify locked cell (worksheet protected)");
            }
        }
    }
}
```

### Ver también

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


