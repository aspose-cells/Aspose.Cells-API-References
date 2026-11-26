---
title: "VbaModuleCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método VbaModuleCollection. Añade un módulo para una hoja de cálculo"
type: docs
url: /es/net/aspose.cells.vba/vbamodulecollection/add/
---
## Add(Worksheet) {#add_1}

Agrega módulo para una hoja de cálculo.

```csharp
public int Add(Worksheet sheet)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| hoja | Hoja de cálculo | La hoja de cálculo |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionMethodAddWithWorksheetDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar un módulo VBA asociado a la hoja de cálculo
            int moduleIndex = workbook.VbaProject.Modules.Add(worksheet);
            
            // Agregar código VBA al módulo
            string vbaCode = "Sub Test()\n    MsgBox \"Hello from VBA!\"\nEnd Sub";
            workbook.VbaProject.Modules[moduleIndex].Codes = vbaCode;
            
            // Guardar el libro con el proyecto VBA
            workbook.Save("output.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Ver también

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)

---

## Add(VbaModuleType, string) {#add}

Agrega módulo.

```csharp
public int Add(VbaModuleType type, string name)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | VbaModuleType | El tipo de módulo. |
| name | String | El nombre del módulo. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionMethodAddWithVbaModuleTypeStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            VbaProject vbaProject = workbook.VbaProject;

            int index = vbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
            VbaModule module = vbaProject.Modules[index];
            module.Codes = "Sub Test()\r\nMsgBox \"Hello World\"\r\nEnd Sub";

            workbook.Save("VbaModuleAddExample.xlsm");
        }
    }
}
```

### Ver también

* enum [VbaModuleType](../../vbamoduletype/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


