---
title: "Enumeración VbaModuleType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Vba.VbaModuleType. Representa el tipo de módulo VBA"
type: docs
url: /es/net/aspose.cells.vba/vbamoduletype/
---
## VbaModuleType enumeration

Representa el tipo de módulo VBA.

```csharp
public enum VbaModuleType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Procedural | `0` | Representa un módulo procedural. |
| Document | `1` | Representa un módulo de documento. |
| Class | `2` | Representa un módulo de clase. |
| Designer | `3` | Representa un módulo de diseñador. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaModuleTypeDemo
    {
        public static void VbaModuleTypeExample()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();
            
            // Inicializar proyecto VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // Agregar un nuevo módulo de clase
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "test");
            
            // Obtener el módulo VBA
            VbaModule vbaModule = vbaProject.Modules[index];
            
            // Establecer códigos para el módulo
            vbaModule.Codes = "Sub ShowMessage()\r\nMsgBox \"Welcome to Aspose!\"\r\nEnd Sub";
            
            // Guardar el archivo Excel
            workbook.Save("VbaModuleTypeExample.xlsm");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


