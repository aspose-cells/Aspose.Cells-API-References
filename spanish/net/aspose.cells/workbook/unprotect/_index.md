---
title: "Workbook.Unprotect"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de Workbook. Desprotege un libro de trabajo"
type: docs
url: /es/net/aspose.cells/workbook/unprotect/
---
## Workbook.Unprotect method

Desprotege un libro de trabajo.

```csharp
public void Unprotect(string password)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| contraseña | String | Contraseña para desproteger el libro de trabajo. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodUnprotectWithStringDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con protección
            Workbook workbook = new Workbook();
            workbook.Protect(ProtectionType.All, "book");

            // Desproteger el libro de trabajo con la contraseña correcta
            workbook.Unprotect("book");

            // Guardar el libro de trabajo desprotegido
            workbook.Save("unprotected_workbook.xlsx");
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


