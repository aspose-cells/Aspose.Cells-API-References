---
title: "WriteProtection.Password"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WriteProtection. Establece la contraseña de protección para modificar el archivo"
type: docs
url: /es/net/aspose.cells/writeprotection/password/
---
## WriteProtection.Password property

Establece la contraseña de protección para modificar el archivo.

```csharp
public string Password { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WriteProtectionPropertyPasswordDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer la contraseña de protección contra escritura
            workbook.Settings.WriteProtection.Password = "owner";
            
            // Guarda el libro de trabajo
            workbook.Save("WriteProtectedWorkbook.xlsx");
            
            Console.WriteLine("Workbook write-protected with password successfully.");
        }
    }
}
```

### Ver también

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


