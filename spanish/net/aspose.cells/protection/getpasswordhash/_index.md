---
title: "Protection.GetPasswordHash"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Protection. Obtiene el hash de la contraseña actual"
type: docs
url: /es/net/aspose.cells/protection/getpasswordhash/
---
## Protection.GetPasswordHash method

Obtiene el hash de la contraseña actual.

```csharp
public int GetPasswordHash()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ProtectionMethodGetPasswordHashDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer la configuración de protección con contraseña
            Protection protection = worksheet.Protection;
            protection.Password = "password123";
            protection.AllowDeletingColumn = true;
            protection.AllowFormattingCell = true;
            
            // Proteger la hoja de cálculo
            worksheet.Protect(ProtectionType.All);

            try
            {
                // Obtener el hash de la contraseña
                int passwordHash = protection.GetPasswordHash();
                
                // Mostrar el resultado
                Console.WriteLine($"Password hash: {passwordHash}");
                Console.WriteLine($"Is protected with password: {protection.IsProtectedWithPassword}");

                // Verificar la contraseña (demostrando la funcionalidad relacionada)
                bool isVerified = protection.VerifyPassword("password123");
                Console.WriteLine($"Password verification result: {isVerified}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetPasswordHash method: {ex.Message}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("ProtectionMethodGetPasswordHashDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


