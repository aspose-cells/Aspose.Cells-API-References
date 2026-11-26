---
title: "VbaModuleCollection.GetDesignerStorage"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método VbaModuleCollection. Representa los datos del Diseñador"
type: docs
url: /es/net/aspose.cells.vba/vbamodulecollection/getdesignerstorage/
---
## VbaModuleCollection.GetDesignerStorage method

Representa los datos del Diseñador.

```csharp
public byte[] GetDesignerStorage(string name)
```

### Observaciones

No admitimos analizarlos. Solo para copiar.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionMethodGetDesignerStorageWithStringDemo
    {
        public static void Run()
        {
            // Crear un libro con proyecto VBA
            Workbook workbook = new Workbook();
            
            // Agregar un módulo de diseñador
            int index = workbook.VbaProject.Modules.Add(VbaModuleType.Designer, "TestForm");
            
            // Obtener el almacenamiento del diseñador (será nulo inicialmente)
            byte[] storage = workbook.VbaProject.Modules.GetDesignerStorage("TestForm");
            Console.WriteLine("Initial designer storage: " + (storage == null ? "null" : "exists"));
            
            // Agregar algunos datos de almacenamiento del diseñador
            byte[] sampleData = new byte[] { 0x01, 0x02, 0x03 };
            workbook.VbaProject.Modules.AddDesignerStorage("TestForm", sampleData);
            
            // Obtener y mostrar el almacenamiento del diseñador
            storage = workbook.VbaProject.Modules.GetDesignerStorage("TestForm");
            Console.WriteLine("Storage after adding: " + (storage == null ? "null" : BitConverter.ToString(storage)));
        }
    }
}
```

### Ver también

* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


