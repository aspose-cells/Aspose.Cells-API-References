---
title: "VbaModuleCollection.AddDesignerStorage"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método VbaModuleCollection."
type: docs
url: /es/net/aspose.cells.vba/vbamodulecollection/adddesignerstorage/
---
## VbaModuleCollection.AddDesignerStorage method

```csharp
public void AddDesignerStorage(string name, byte[] data)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String |  |
| datos | Byte[] |  |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;
    using System.Text;

    public class VbaModuleCollectionMethodAddDesignerStorageWithStringByteDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder al proyecto VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // Preparar datos para el almacenamiento del diseñador
            string storageName = "MyDesignerStorage";
            byte[] storageData = Encoding.UTF8.GetBytes("This is designer storage data");
            
            try
            {
                // Llamar al método AddDesignerStorage
                vbaProject.Modules.AddDesignerStorage(storageName, storageData);
                
                Console.WriteLine("Designer storage added successfully");
                
                // Verificar que el almacenamiento se haya añadido
                byte[] retrievedData = vbaProject.Modules.GetDesignerStorage(storageName);
                if (retrievedData != null)
                {
                    Console.WriteLine("Retrieved storage data: " + Encoding.UTF8.GetString(retrievedData));
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddDesignerStorage method: {ex.Message}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("VbaModuleCollectionMethodAddDesignerStorageWithStringByteDemo.xlsx");
        }
    }
}
```

### Ver también

* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


