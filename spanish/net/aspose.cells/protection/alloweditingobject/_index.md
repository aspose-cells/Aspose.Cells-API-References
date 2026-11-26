---
title: "Protection.AllowEditingObject"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Protection property. Representa si el usuario tiene permiso para manipular objetos de dibujo en una hoja de cálculo protegida"
type: docs
url: /es/net/aspose.cells/protection/alloweditingobject/
---
## Protection.AllowEditingObject property

Representa si se permite al usuario manipular objetos de dibujo en una hoja de cálculo protegida.

```csharp
public bool AllowEditingObject { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowEditingObjectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Configura la protección con AllowEditingObject habilitado
            Protection protection = worksheet.Protection;
            protection.AllowEditingObject = true;
            protection.AllowEditingContent = false; // Contrast with AllowEditingObject
            worksheet.Protect(ProtectionType.All);

            // Verifica las banderas de protección
            Console.WriteLine("Protection Settings:");
            Console.WriteLine($"AllowEditingObject: {protection.AllowEditingObject}");
            Console.WriteLine($"AllowEditingContent: {protection.AllowEditingContent}");

            // Crea un cuadro de texto (objeto) para probar la edición
            worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            
            // Guarda el libro de trabajo
            workbook.Save("ProtectionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


