---
title: "VbaModule.Codes"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad VbaModule. Obtiene y establece los códigos del módulo"
type: docs
url: /es/net/aspose.cells.vba/vbamodule/codes/
---
## VbaModule.Codes property

Obtiene y establece los códigos del módulo.

```csharp
public string Codes { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModulePropertyCodesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar un módulo VBA
            int index = workbook.VbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
            Aspose.Cells.Vba.VbaModule module = workbook.VbaProject.Modules[index];
            
            // Establecer código inicial
            module.Codes = "Sub TestMacro()\n    MsgBox \"Hello World\"\nEnd Sub";
            
            // Modificar el código añadiendo nuevas líneas
            module.Codes = module.Codes + "\nSub AnotherMacro()\n    MsgBox \"Second Macro\"\nEnd Sub";
            
            // Guarda el libro de trabajo
            workbook.Save("VbaModuleDemo.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Ver también

* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


