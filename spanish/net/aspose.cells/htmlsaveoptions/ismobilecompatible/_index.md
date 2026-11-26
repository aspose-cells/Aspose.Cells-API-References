---
title: "HtmlSaveOptions.IsMobileCompatible"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si el HTML de salida es compatible con dispositivos móviles. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/ismobilecompatible/
---
## HtmlSaveOptions.IsMobileCompatible property

Indica si el HTML de salida es compatible con dispositivos móviles. El valor predeterminado es false.

```csharp
public bool IsMobileCompatible { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsMobileCompatibleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Mobile Compatibility Test");

            // Crear opciones de guardado HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Establecer compatibilidad móvil
            saveOptions.IsMobileCompatible = true;

            // Guardar con compatibilidad móvil habilitada
            workbook.Save("MobileCompatible.html", saveOptions);

            // Cambiar a no compatible con móviles
            saveOptions.IsMobileCompatible = false;
            workbook.Save("NonMobileCompatible.html", saveOptions);
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


