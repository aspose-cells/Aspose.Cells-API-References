---
title: "Clase ProtectedRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.ProtectedRange. Un rango especificado que se permite editar cuando la protección de la hoja está ACTIVADA"
type: docs
url: /es/net/aspose.cells/protectedrange/
---
## ProtectedRange class

Un rango especificado que se permite editar cuando la protección de la hoja está ACTIVADA.

```csharp
public class ProtectedRange
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CellArea](../../aspose.cells/protectedrange/cellarea/) { get; } | Obtiene el objeto [`CellArea`](./cellarea/) que representa el área de celdas a proteger. |
| [IsProtectedWithPassword](../../aspose.cells/protectedrange/isprotectedwithpassword/) { get; } | Indica si la hoja de cálculo está protegida con contraseña. |
| [Name](../../aspose.cells/protectedrange/name/) { get; set; } | Obtiene el título del rango. Se usa como descriptor, no como una definición de rango con nombre. |
| [Password](../../aspose.cells/protectedrange/password/) { get; set; } | Representa la contraseña para proteger el rango. |
| [SecurityDescriptor](../../aspose.cells/protectedrange/securitydescriptor/) { get; set; } | El descriptor de seguridad define las cuentas de usuario que pueden editar este rango sin proporcionar una contraseña para acceder al rango. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AddArea](../../aspose.cells/protectedrange/addarea/)(int, int, int, int) | Agrega un área referida a este |
| [GetAreas](../../aspose.cells/protectedrange/getareas/)() | Obtiene todas las áreas referidas. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassProtectedRangeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtén la colección de rangos protegidos
            ProtectedRangeCollection protectedRanges = worksheet.AllowEditRanges;
            
            // Agregar un nuevo rango protegido (A1:J10)
            int index = protectedRanges.Add("MyProtectedRange", 0, 0, 10, 10);
            
            // Obtener el rango protegido
            ProtectedRange protectedRange = protectedRanges[index];
            
            // Establecer descriptor de seguridad
            string securityDescriptor = "O:WDG:WDD:(D;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1000)(A;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1013)";
            protectedRange.SecurityDescriptor = securityDescriptor;
            
            // Guarda el libro de trabajo
            workbook.Save("ProtectedRangeDemo.xlsx");
            
            Console.WriteLine("Protected range demo completed successfully.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


