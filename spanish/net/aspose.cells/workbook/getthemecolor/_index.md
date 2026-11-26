---
title: "Workbook.GetThemeColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Workbook. Obtiene el color del tema"
type: docs
url: /es/net/aspose.cells/workbook/getthemecolor/
---
## Workbook.GetThemeColor method

Obtiene el color del tema.

```csharp
public Color GetThemeColor(ThemeColorType type)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | ThemeColorType | El tipo de color del tema. |

### Valor de retorno

El color del tema.

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodGetThemeColorWithThemeColorTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Obtener el color del tema para Accent6
            Color color = workbook.GetThemeColor(ThemeColorType.Accent6);
            Console.WriteLine("Theme Color (Accent6): " + color.ToString());
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* enum [ThemeColorType](../../themecolortype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


