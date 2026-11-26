---
title: "Protection.AllowEditingContent"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Protection. Representa si el usuario puede editar el contenido de celdas bloqueadas en una hoja de cálculo protegida"
type: docs
url: /es/net/aspose.cells/protection/alloweditingcontent/
---
## Protection.AllowEditingContent property

Representa si se permite al usuario editar el contenido de celdas bloqueadas en una hoja de cálculo protegida.

```csharp
public bool AllowEditingContent { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowEditingContentDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Proteger la hoja de cálculo con una contraseña
            worksheet.Protect(ProtectionType.All, "password", null);
            
            // Comprobar y mostrar la propiedad AllowEditingContent
            Console.WriteLine("AllowEditingContent before setting: " + worksheet.Protection.AllowEditingContent);
            
            // Modificar la propiedad AllowEditingContent
            worksheet.Protection.AllowEditingContent = true;
            
            // Comprobar y mostrar la propiedad actualizada
            Console.WriteLine("AllowEditingContent after setting: " + worksheet.Protection.AllowEditingContent);
            
            // Guarda el libro de trabajo
            workbook.Save("ProtectionPropertyAllowEditingContentDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


