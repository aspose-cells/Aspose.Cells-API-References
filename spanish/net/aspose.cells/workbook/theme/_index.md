---
title: "Workbook.Theme"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad del libro de trabajo. Obtiene el nombre del tema"
type: docs
url: /es/net/aspose.cells/workbook/theme/
---
## Workbook.Theme property

Obtiene el nombre del tema.

```csharp
public string Theme { get; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyThemeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Demostrar la obtención del tema predeterminado
            Console.WriteLine("Default theme: " + workbook.Theme);
            
            // Cambiar el color del tema y verificar
            workbook.SetThemeColor(ThemeColorType.Accent1, Color.Blue);
            Color accent1 = workbook.GetThemeColor(ThemeColorType.Accent1);
            Console.WriteLine("Modified Accent1 color: " + accent1);
            
            // Guardar el libro de trabajo para demostrar la persistencia del tema
            workbook.Save("ThemeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


