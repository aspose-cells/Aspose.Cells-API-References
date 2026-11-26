---
title: "VbaProject.IsProtected"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad VbaProject. Indica si este proyecto VBA está protegido"
type: docs
url: /es/net/aspose.cells.vba/vbaproject/isprotected/
---
## VbaProject.IsProtected property

Indica si este proyecto VBA está protegido.

```csharp
public bool IsProtected { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyIsProtectedDemo
    {
        public static void Run()
        {
            // Cargar un archivo de Excel de ejemplo con proyecto VBA sin protección
            Workbook wb = new Workbook("load.xlsm");
            VbaProject vbaProject = wb.VbaProject;
            Console.WriteLine("Is VBA Project Protected (load.xlsm): " + vbaProject.IsProtected);
            Console.WriteLine("Is VBA Project Locked for Viewing: " + vbaProject.IslockedForViewing);

            // Cargar un archivo de Excel de ejemplo con proyecto VBA protegido
            wb = new Workbook("load_protected.xlsm");
            vbaProject = wb.VbaProject;
            Console.WriteLine("Is VBA Project Protected (load_protected.xlsm): " + vbaProject.IsProtected);
            Console.WriteLine("Is VBA Project Locked for Viewing: " + vbaProject.IslockedForViewing);

            // Cargar un archivo de Excel de ejemplo con proyecto VBA protegido y bloqueado
            wb = new Workbook("load_protected_lockedForView.xlsm");
            vbaProject = wb.VbaProject;
            Console.WriteLine("Is VBA Project Protected (load_protected_lockedForView.xlsm): " + vbaProject.IsProtected);
            Console.WriteLine("Is VBA Project Locked for Viewing: " + vbaProject.IslockedForViewing);
        }
    }
}
```

### Ver también

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


