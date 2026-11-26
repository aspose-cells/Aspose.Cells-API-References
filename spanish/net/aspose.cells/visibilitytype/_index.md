---
title: "Enum VisibilityType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.VisibilityType. Representa los estados de visibilidad de la hoja"
type: docs
url: /es/net/aspose.cells/visibilitytype/
---
## VisibilityType enumeration

Representa los estados de la visibilidad de la hoja.

```csharp
public enum VisibilityType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Visible | `0` | Indica que la hoja está visible. |
| Hidden | `1` | Indica que la hoja está oculta, pero puede ser mostrada por el usuario a través de la interfaz de usuario. |
| VeryHidden | `2` | Indica que la hoja está oculta y no puede mostrarse en la interfaz de usuario (UI). Este estado solo está disponible programáticamente. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class VisibilityTypeDemo
    {
        public static void VisibilityTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("NewSheet");
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer el nombre de la hoja de cálculo
            worksheet.Name = "DemoSheet";

            // Establecer la visibilidad de la hoja de cálculo como Oculta
            worksheet.VisibilityType = VisibilityType.Hidden;

            // Guarda el libro de trabajo
            workbook.Save("VisibilityTypeExample.xlsx");

            // Salida para indicar que el proceso ha finalizado
            Console.WriteLine("Workbook saved with the worksheet visibility set to Hidden.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


