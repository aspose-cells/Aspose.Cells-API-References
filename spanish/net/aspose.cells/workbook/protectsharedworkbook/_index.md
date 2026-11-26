---
title: "Workbook.ProtectSharedWorkbook"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Workbook. Protege un libro de trabajo compartido"
type: docs
url: /es/net/aspose.cells/workbook/protectsharedworkbook/
---
## Workbook.ProtectSharedWorkbook method

Protege un libro de trabajo compartido.

```csharp
public void ProtectSharedWorkbook(string password)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| contraseña | String | Contraseña para proteger el libro de trabajo. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodProtectSharedWorkbookWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook wb = new Workbook();
            
            // Proteger el libro de trabajo compartido con contraseña
            wb.ProtectSharedWorkbook("abcd");
            
            // Guardar el libro de trabajo protegido
            wb.Save("ProtectedSharedWorkbook.xlsx");
            
            // Cargar el libro de trabajo protegido
            Workbook wbProtected = new Workbook("ProtectedSharedWorkbook.xlsx");
            
            // Verificar el estado de protección
            Console.WriteLine("Workbook is protected: " + wbProtected.Settings.IsProtected);
            
            // Desproteger el libro de trabajo
            wbProtected.UnprotectSharedWorkbook("abcd");
            
            // Guardar el libro de trabajo desprotegido
            wbProtected.Save("UnprotectedSharedWorkbook.xlsx");
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


