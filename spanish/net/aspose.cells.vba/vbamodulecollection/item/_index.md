---
title: "VbaModuleCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad VbaModuleCollection. Obtiene VbaModule en la lista por el índice"
type: docs
url: /es/net/aspose.cells.vba/vbamodulecollection/item/
---
## VbaModuleCollection indexer (1 of 2)

Obtiene [`VbaModule`](../../vbamodule/) en la lista por el índice.

```csharp
public VbaModule this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con proyecto VBA
            Workbook workbook = new Workbook("sample.xlsm");
            
            // Obtener proyecto VBA existente (VbaProject es de solo lectura)
            VbaProject vbaProject = workbook.VbaProject;
            
            // Agregar un módulo al proyecto VBA
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
            
            // Acceder al módulo usando la propiedad Item
            VbaModule module = vbaProject.Modules[index];
            
            // Agregar código VBA al módulo
            module.Codes = "Sub TestMacro()\n    MsgBox \"Hello from VBA!\"\nEnd Sub";
            
            // Guarda el libro de trabajo
            workbook.Save("VbaModuleDemo.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Ver también

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)

---

## VbaModuleCollection indexer (2 of 2)

Obtiene [`VbaModule`](../../vbamodule/) en la lista por el nombre.

```csharp
public VbaModule this[string name] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| name | El nombre del módulo. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar módulo VBA al libro de trabajo
            int moduleIndex = workbook.VbaProject.Modules.Add(worksheet);
            
            // Acceder al módulo usando la propiedad Item por nombre
            VbaModule module = workbook.VbaProject.Modules[worksheet.CodeName];
            
            // Establecer código VBA
            module.Codes = "Sub Test()\r\n    MsgBox \"Hello World!\"\r\nEnd Sub";
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsm", SaveFormat.Xlsm);
            
            // Verificar cargando nuevamente
            Workbook verifyWorkbook = new Workbook("output.xlsm");
            VbaModule verifyModule = verifyWorkbook.VbaProject.Modules[worksheet.CodeName];
            
            Console.WriteLine("VBA Code in saved file:");
            Console.WriteLine(verifyModule.Codes);
        }
    }
}
```

### Ver también

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


