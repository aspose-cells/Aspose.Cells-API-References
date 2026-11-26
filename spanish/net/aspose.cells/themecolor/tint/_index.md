---
title: "ThemeColor.Tint"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ThemeColor. Obtiene y establece el valor del tinte"
type: docs
url: /es/net/aspose.cells/themecolor/tint/
---
## ThemeColor.Tint property

Obtiene y establece el valor de tono.

```csharp
public double Tint { get; set; }
```

### Observaciones

El valor del tinte se almacena como un double de -1.0 a 1.0, donde -1.0 significa 100% oscurecer y 1.0 significa 100% aclarar. Además, 0.0 significa sin cambios.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThemeColorPropertyTintDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un estilo con color temático y tinte
            Style style = workbook.CreateStyle();
            style.BackgroundThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5); // 0.5 tint
            
            // Aplicar el estilo a una celda
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);

            // Obtener el valor del tinte del estilo de la celda
            double tintValue = cell.GetStyle().BackgroundThemeColor.Tint;
            Console.WriteLine("Tint value: " + tintValue);

            // Modificar el valor del tinte
            ThemeColor themeColor = cell.GetStyle().BackgroundThemeColor;
            themeColor.Tint = 0.8; // Change tint to 0.8
            cell.SetStyle(style);

            // Verificar el nuevo valor del tinte
            Console.WriteLine("Modified tint value: " + cell.GetStyle().BackgroundThemeColor.Tint);
        }
    }
}
```

### Ver también

* class [ThemeColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


