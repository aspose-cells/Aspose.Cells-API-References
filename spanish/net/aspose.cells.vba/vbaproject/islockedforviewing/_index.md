---
title: "VbaProject.IslockedForViewing"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad VbaProject. Indica si este proyecto VBA está bloqueado para visualización"
type: docs
url: /es/net/aspose.cells.vba/vbaproject/islockedforviewing/
---
## VbaProject.IslockedForViewing property

Indica si este proyecto VBA está bloqueado para visualización.

```csharp
[Obsolete("Use VbaProject.IsLockedForView property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IslockedForViewing { get; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad VbaProject.IsLockedForView. Esta propiedad será eliminada 12 meses después a partir de julio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyIslockedForViewingDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de ejemplo con proyecto VBA
            Workbook wb = new Workbook();
            // Crear una nueva hoja de cálculo para asegurar que el proyecto VBA se cree
            wb.Worksheets.Add();
            
            // Demostrar la propiedad IslockedForViewing
            Console.WriteLine("Initial state:");
            Console.WriteLine($"IsProtected: {wb.VbaProject.IsProtected}");
            Console.WriteLine($"IslockedForViewing: {wb.VbaProject.IslockedForViewing}\n");

            // Proteger y bloquear para visualización
            wb.VbaProject.Protect(true, "password123");
            Console.WriteLine("After protecting and locking for viewing:");
            Console.WriteLine($"IsProtected: {wb.VbaProject.IsProtected}");
            Console.WriteLine($"IslockedForViewing: {wb.VbaProject.IslockedForViewing}\n");

            // Proteger sin bloquear para visualización
            wb.VbaProject.Protect(false, "password456");
            Console.WriteLine("After protecting without locking for viewing:");
            Console.WriteLine($"IsProtected: {wb.VbaProject.IsProtected}");
            Console.WriteLine($"IslockedForViewing: {wb.VbaProject.IslockedForViewing}\n");

            // Eliminar protección
            wb.VbaProject.Protect(true, "");
            Console.WriteLine("After removing protection:");
            Console.WriteLine($"IsProtected: {wb.VbaProject.IsProtected}");
            Console.WriteLine($"IslockedForViewing: {wb.VbaProject.IslockedForViewing}");
        }
    }
}
```

### Ver también

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


