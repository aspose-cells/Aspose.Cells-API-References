---
title: "Protection.IsProtectedWithPassword"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Protection. Indica si la hoja de cálculo está protegida con contraseña"
type: docs
url: /es/net/aspose.cells/protection/isprotectedwithpassword/
---
## Protection.IsProtectedWithPassword property

Indica si la hoja de cálculo está protegida con contraseña.

```csharp
public bool IsProtectedWithPassword { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyIsProtectedWithPasswordDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accede a la configuración de protección de la hoja de cálculo
            Protection protection = worksheet.Protection;

            // Establecer la contraseña de protección
            protection.Password = "test123";

            // Comprobar si la hoja de cálculo está protegida con contraseña
            bool isProtectedWithPassword = protection.IsProtectedWithPassword;
            Console.WriteLine("Is worksheet protected with password: " + isProtectedWithPassword);

            // Guarda el libro de trabajo
            workbook.Save("PasswordProtectionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


