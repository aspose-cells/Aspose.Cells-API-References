---
title: "Protection.Password"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Protection. Representa la contraseña para proteger la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/protection/password/
---
## Protection.Password property

Representa la contraseña para proteger la hoja de cálculo.

```csharp
public string Password { get; set; }
```

### Observaciones

Si la contraseña se establece en null o cadena vacía, puedes desproteger la hoja de cálculo o el libro sin usar una contraseña. De lo contrario, debes especificar la contraseña para desproteger la hoja de cálculo o el libro.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyPasswordDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer la configuración de protección con contraseña
            Protection protection = worksheet.Protection;
            protection.AllowEditingContent = false;
            protection.AllowDeletingColumn = false;
            protection.Password = "test123";

            // Verificar la protección con contraseña
            Console.WriteLine("Worksheet is protected: " + (protection.Password != null));
            Console.WriteLine("Protection password: " + protection.Password);

            // Crear otro objeto de protección para comparar
            Protection protection2 = worksheet.Protection;
            protection2.Password = "test123";

            // Comparar la protección con contraseña
            Console.WriteLine("Passwords match: " + (protection.Password == protection2.Password));
        }
    }
}
```

### Ver también

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


