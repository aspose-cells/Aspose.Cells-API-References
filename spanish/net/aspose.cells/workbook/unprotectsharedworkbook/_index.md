---
title: "Workbook.UnprotectSharedWorkbook"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Workbook. Desprotege un libro de trabajo compartido"
type: docs
url: /es/net/aspose.cells/workbook/unprotectsharedworkbook/
---
## Workbook.UnprotectSharedWorkbook method

Desprotege un libro de trabajo compartido.

```csharp
public void UnprotectSharedWorkbook(string password)
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
    public class WorkbookMethodUnprotectSharedWorkbookWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook wb = new Workbook();
            
            // Proteger el libro de trabajo compartido con contraseña
            wb.ProtectSharedWorkbook("abcd");
            
            // Guardar el libro de trabajo protegido
            wb.Save("ProtectedSharedWorkbook.xlsx");
            
            // Reabrir el libro de trabajo
            wb = new Workbook("ProtectedSharedWorkbook.xlsx");
            
            // Desproteger el libro de trabajo compartido con contraseña
            wb.UnprotectSharedWorkbook("abcd");
            
            // Guardar el libro de trabajo desprotegido
            wb.Save("UnprotectedSharedWorkbook.xlsx");
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


