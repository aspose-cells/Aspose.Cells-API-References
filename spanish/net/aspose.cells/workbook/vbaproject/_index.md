---
title: "Workbook.VbaProject"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Workbook. Obtiene el VbaProject en una hoja de cálculo"
type: docs
url: /es/net/aspose.cells/workbook/vbaproject/
---
## Workbook.VbaProject property

Obtiene el `VbaProject` en una hoja de cálculo.

```csharp
public VbaProject VbaProject { get; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyVbaProjectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceda al proyecto VBA (VbaProject es de solo lectura, solo podemos comprobar si existe)
            if (workbook.VbaProject == null)
            {
                // Cree un proyecto VBA guardando como libro de trabajo con macros habilitadas
                workbook.Save("temp.xlsm", SaveFormat.Xlsm);
                workbook = new Workbook("temp.xlsm");
                File.Delete("temp.xlsm");
            }

            // Agregue un nuevo módulo al proyecto VBA
            int moduleIndex = workbook.VbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
            
            // Obtenga el módulo agregado y establezca su código
            VbaModule module = workbook.VbaProject.Modules[moduleIndex];
            module.Codes = "Sub Test()\r\n    MsgBox \"Hello from VBA!\"\r\nEnd Sub";

            // Guarda el libro de trabajo
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "VbaProjectDemo.xlsm");
            workbook.Save(outputPath, SaveFormat.Xlsm);
        }
    }
}
```

### Ver también

* class [VbaProject](../../../aspose.cells.vba/vbaproject/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


