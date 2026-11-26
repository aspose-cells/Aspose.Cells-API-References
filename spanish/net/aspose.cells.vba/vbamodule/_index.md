---
title: "Clase VbaModule"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Vba.VbaModule. Representa el módulo en el proyecto VBA"
type: docs
url: /es/net/aspose.cells.vba/vbamodule/
---
## VbaModule class

Representa el módulo en el proyecto VBA.

```csharp
public class VbaModule
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BinaryCodes](../../aspose.cells.vba/vbamodule/binarycodes/) { get; } | Obtiene y establece los códigos binarios del módulo. |
| [Codes](../../aspose.cells.vba/vbamodule/codes/) { get; set; } | Obtiene y establece los códigos del módulo. |
| [Name](../../aspose.cells.vba/vbamodule/name/) { get; set; } | Obtiene y establece el nombre del módulo. |
| [Type](../../aspose.cells.vba/vbamodule/type/) { get; } | Obtiene el tipo del módulo. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaModuleDemo
    {
        public static void VbaModuleExample()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();

            // Inicializar proyecto VBA
            VbaProject vbaProject = workbook.VbaProject;

            // Agregar un nuevo módulo
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "test");

            // Obtener el módulo VBA
            VbaModule vbaModule = vbaProject.Modules[index];

            // Establecer los códigos para el módulo
            vbaModule.Codes = "Sub ShowMessage()\r\nMsgBox \"Welcome to Aspose!\"\r\nEnd Sub";

            // Guardando el archivo Excel
            workbook.Save("VbaModuleExample.xlsm");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


