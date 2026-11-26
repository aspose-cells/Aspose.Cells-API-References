---
title: "Workbook.Protect"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método del libro de trabajo. Protege un libro de trabajo"
type: docs
url: /es/net/aspose.cells/workbook/protect/
---
## Workbook.Protect method

Protege un libro de trabajo.

```csharp
public void Protect(ProtectionType protectionType, string password)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| protectionType | ProtectionType | Tipo de protección. |
| contraseña | String | Contraseña para proteger el libro de trabajo. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodProtectWithProtectionTypeStringDemo
    {
        public static void Run()
        {
            Workbook wbk = new Workbook();
            wbk.Protect(ProtectionType.Structure, "password123");
            
            wbk.Save("protected_workbook.xlsx", SaveFormat.Xlsx);
            wbk.Dispose();
        }
    }
}
```

### Ver también

* enum [ProtectionType](../../protectiontype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


