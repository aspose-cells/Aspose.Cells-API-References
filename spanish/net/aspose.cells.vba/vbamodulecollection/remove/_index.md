---
title: "VbaModuleCollection.Remove"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método VbaModuleCollection. Elimina un módulo para una hoja de cálculo"
type: docs
url: /es/net/aspose.cells.vba/vbamodulecollection/remove/
---
## Remove(Worksheet) {#remove}

Elimina módulo para una hoja de cálculo.

```csharp
public void Remove(Worksheet sheet)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| hoja | Hoja de cálculo | La hoja de cálculo |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaModuleCollectionMethodRemoveWithWorksheetDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar un módulo VBA a la hoja de cálculo
            int moduleIndex = workbook.VbaProject.Modules.Add(worksheet);
            
            // Obtener la colección de módulos VBA
            VbaModuleCollection modules = workbook.VbaProject.Modules;
            
            try
            {
                // Llamar al método Remove con el parámetro de hoja de cálculo
                modules.Remove(worksheet);
                
                Console.WriteLine("VBA module removed successfully for the specified worksheet.");
                
                // Verifique que el módulo se eliminó
                if (modules.Count == 0)
                {
                    Console.WriteLine("No VBA modules remain in the collection.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Remove method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("VbaModuleRemoveWithWorksheetDemo.xlsx");
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

## Remove(string) {#remove_1}

Eliminar el módulo por el nombre

```csharp
public void Remove(string name)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String |  |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionMethodRemoveWithStringDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con macro
            Workbook workbook = new Workbook();
            
            // Acceder al proyecto VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // Agregar un nuevo módulo
            int index = vbaProject.Modules.Add(VbaModuleType.Procedural, "TestModule");
            
            // Agregar código al módulo
            vbaProject.Modules[index].Codes = "Sub Test()\r\nMsgBox \"Hello World\"\r\nEnd Sub";
            
            // Guarda el libro de trabajo
            workbook.Save("output_with_module.xlsm");
            
            // Eliminar el módulo por nombre
            vbaProject.Modules.Remove("TestModule");
            
            // Guardar el libro de trabajo después de la eliminación
            workbook.Save("output_after_removal.xlsm");
        }
    }
}
```

### Ver también

* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


