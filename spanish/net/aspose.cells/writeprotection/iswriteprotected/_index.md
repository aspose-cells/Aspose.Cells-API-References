---
title: "WriteProtection.IsWriteProtected"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WriteProtection. Indica si este libro de trabajo está protegido contra escritura"
type: docs
url: /es/net/aspose.cells/writeprotection/iswriteprotected/
---
## WriteProtection.IsWriteProtected property

Indica si este libro de trabajo está protegido contra escritura.

```csharp
public bool IsWriteProtected { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WriteProtectionPropertyIsWriteProtectedDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Habilitar la protección contra escritura con contraseña
            workbook.Settings.WriteProtection.Password = "1234";
            
            // Comprobar si el libro de trabajo está protegido contra escritura
            Console.WriteLine("Is workbook write protected? " + 
                workbook.Settings.WriteProtection.IsWriteProtected);
            
            // Validar la contraseña
            Console.WriteLine("Is password valid? " + 
                workbook.Settings.WriteProtection.ValidatePassword("1234"));
            
            // Guarda el libro de trabajo
            workbook.Save("WriteProtectedWorkbook.xlsx");
            
            // Cargar el libro de trabajo guardado para verificar la protección
            Workbook loadedWorkbook = new Workbook("WriteProtectedWorkbook.xlsx");
            
            // Verificar el estado de la protección nuevamente
            Console.WriteLine("Is loaded workbook write protected? " + 
                loadedWorkbook.Settings.WriteProtection.IsWriteProtected);
        }
    }
}
```

### Ver también

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


