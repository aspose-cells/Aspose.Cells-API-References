---
title: "VbaProject.Modules"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad VbaProject. Obtiene todos los objetos VbaModule"
type: docs
url: /es/net/aspose.cells.vba/vbaproject/modules/
---
## VbaProject.Modules property

Obtiene todos los objetos [`VbaModule`](../../vbamodule/).

```csharp
public VbaModuleCollection Modules { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyModulesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            VbaProject vbaProject = workbook.VbaProject;
            
            // Agregar un nuevo módulo y obtenerlo usando la propiedad Modules
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
            VbaModule module = vbaProject.Modules[index];
            
            // Agregar código al módulo
            module.Codes = "Sub Test()\r\n    MsgBox \"Module demonstration\"\r\nEnd Sub";
            
            // Guardar con formato habilitado para macros
            workbook.Save("VbaModulesDemo.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Ver también

* class [VbaModuleCollection](../../vbamodulecollection/)
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


