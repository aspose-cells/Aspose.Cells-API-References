---
title: "Worksheet.Protect"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Worksheet método. Protege la hoja"
type: docs
url: /es/net/aspose.cells/worksheet/protect/
---
## Protect(ProtectionType) {#protect}

Protege la hoja de cálculo.

```csharp
public void Protect(ProtectionType type)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | ProtectionType | Tipo de protección. |

### Observaciones

Este método protege la hoja sin contraseña. Puede proteger la hoja en todas las versiones del archivo de Excel.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodProtectWithProtectionTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet sheet = workbook.Worksheets[0];
            
            // Protege la hoja con el tipo de protección Objects
            sheet.Protect(ProtectionType.Objects);
            
            // Guarda el libro de trabajo
            workbook.Save("ProtectedWorksheet.xlsx");
        }
    }
}
```

### Ver también

* enum [ProtectionType](../../protectiontype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Protect(ProtectionType, string, string) {#protect_1}

Protege la hoja de cálculo.

```csharp
public void Protect(ProtectionType type, string password, string oldPassword)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | ProtectionType | Tipo de protección. |
| contraseña | String | Contraseña. |
| oldPassword | String | Si la hoja ya está protegida con una contraseña, por favor proporciona la contraseña anterior. De lo contrario, puedes establecer un valor nulo o una cadena vacía en este parámetro. |

### Observaciones

Este método puede proteger la hoja de cálculo en todas las versiones del archivo de Excel.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodProtectWithProtectionTypeStringStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Proteja la hoja de cálculo con contraseña y permita todos los tipos de protección
            worksheet.Protect(ProtectionType.All, "password123", null);
            
            // Guarda el libro de trabajo
            workbook.Save("ProtectedWorksheet.xlsx");
        }
    }
}
```

### Ver también

* enum [ProtectionType](../../protectiontype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


