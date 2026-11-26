---
title: "DefaultStyleSettings.FontSize"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "propiedad DefaultStyleSettings. Obtiene/Establece el tamaño de fuente estándar predeterminado para el libro de trabajo"
type: docs
url: /es/net/aspose.cells/defaultstylesettings/fontsize/
---
## DefaultStyleSettings.FontSize property

Obtiene/Establece el tamaño de fuente estándar predeterminado para el libro de trabajo.

```csharp
public double FontSize { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DefaultStyleSettingsPropertyFontSizeDemo
    {
        public static void Run()
        {
            HtmlLoadOptions htmlLoadOptions = new HtmlLoadOptions();
            
            // Establecer el nombre y tamaño de fuente predeterminados
            htmlLoadOptions.DefaultStyleSettings.FontName = "Calibri";
            htmlLoadOptions.DefaultStyleSettings.FontSize = 11.0;

            // Cargar archivo HTML con estas configuraciones
            Workbook workbook = new Workbook("example.html", htmlLoadOptions);

            // Acceda a una celda y muestre su tamaño de fuente
            Cell cell = workbook.Worksheets[0].Cells["A1"];
            Console.WriteLine("Cell A1 Font Size: " + cell.GetStyle().Font.Size);
        }
    }
}
```

### Ver también

* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


