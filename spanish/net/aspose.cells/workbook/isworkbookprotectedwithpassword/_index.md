---
title: "Workbook.IsWorkbookProtectedWithPassword"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Workbook. Indica si la estructura o la ventana están protegidas con contraseña"
type: docs
url: /es/net/aspose.cells/workbook/isworkbookprotectedwithpassword/
---
## Workbook.IsWorkbookProtectedWithPassword property

Indica si la estructura o la ventana están protegidas con contraseña.

```csharp
public bool IsWorkbookProtectedWithPassword { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyIsWorkbookProtectedWithPasswordDemo
    {
        public static void Run()
        {
            // Crear una nueva instancia de Workbook
            Workbook workbook = new Workbook();

            // Verificar si el libro de trabajo está protegido con contraseña (debe ser falso para un libro de trabajo nuevo)
            Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);

            // Proteger el libro de trabajo con una contraseña
            workbook.Protect(ProtectionType.All, "password123");

            // Ahora verificar de nuevo (debe ser verdadero)
            Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);

            // Desproteger el libro de trabajo
            workbook.Unprotect("password123");

            // Verificación final (debe ser falso de nuevo)
            Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);

            // Liberar el libro de trabajo
            workbook.Dispose();
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


