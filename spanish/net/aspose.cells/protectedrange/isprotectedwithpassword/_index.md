---
title: "ProtectedRange.IsProtectedWithPassword"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ProtectedRange. Indica si la hoja de cálculo está protegida con contraseña"
type: docs
url: /es/net/aspose.cells/protectedrange/isprotectedwithpassword/
---
## ProtectedRange.IsProtectedWithPassword property

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
    public class ProtectedRangePropertyIsProtectedWithPasswordDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear rangos protegidos y obtener sus índices
            int protectedIndex = worksheet.AllowEditRanges.Add("PasswordProtected", 0, 0, 5, 5);
            ProtectedRange protectedWithPassword = worksheet.AllowEditRanges[protectedIndex];
            protectedWithPassword.Password = "test123";
            
            int unprotectedIndex = worksheet.AllowEditRanges.Add("Unprotected", 6, 0, 11, 5);
            ProtectedRange unprotected = worksheet.AllowEditRanges[unprotectedIndex];
            
            // Proteger la hoja de cálculo para aplicar restricciones
            worksheet.Protect(ProtectionType.All);
            
            // Verificar el estado de protección con contraseña
            Console.WriteLine($"Range '{protectedWithPassword.Name}' password protected: {protectedWithPassword.IsProtectedWithPassword}");
            Console.WriteLine($"Range '{unprotected.Name}' password protected: {unprotected.IsProtectedWithPassword}");
        }
    }
}
```

### Ver también

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


