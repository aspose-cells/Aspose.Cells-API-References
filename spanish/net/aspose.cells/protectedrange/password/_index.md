---
title: "ProtectedRange.Password"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ProtectedRange. Representa la contraseña para proteger el rango"
type: docs
url: /es/net/aspose.cells/protectedrange/password/
---
## ProtectedRange.Password property

Representa la contraseña para proteger el rango.

```csharp
public string Password { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangePropertyPasswordDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear colección de rangos protegidos
            ProtectedRangeCollection allowRanges = worksheet.AllowEditRanges;

            // Agregar un rango protegido
            int index = allowRanges.Add("MyProtectedRange", 0, 0, 2, 2);
            ProtectedRange protectedRange = allowRanges[index];

            // Establecer contraseña para el rango protegido
            protectedRange.Password = "12345";

            // Guarda el libro de trabajo
            workbook.Save("ProtectedRangeWithPassword.xlsx");
        }
    }
}
```

### Ver también

* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


