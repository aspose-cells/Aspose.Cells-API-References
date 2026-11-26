---
title: "DefaultStyleSettings.HorizontalAlignment"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DefaultStyleSettings. Gets/Sets el valor predeterminado para la alineación horizontal"
type: docs
url: /es/net/aspose.cells/defaultstylesettings/horizontalalignment/
---
## DefaultStyleSettings.HorizontalAlignment property

Obtiene/Establece el valor predeterminado para la alineación horizontal

```csharp
public TextAlignmentType HorizontalAlignment { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DefaultStyleSettingsPropertyHorizontalAlignmentDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            DefaultStyleSettings defaultStyleSettings = workbook.Settings.DefaultStyleSettings;

            // Establezca la alineación horizontal para demostrar la propiedad
            defaultStyleSettings.HorizontalAlignment = TextAlignmentType.Center;

            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Centered Text";
            worksheet.Cells.ApplyStyle(workbook.CreateStyle(), new StyleFlag() { All = true });

            workbook.Save("HorizontalAlignmentDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [TextAlignmentType](../../textalignmenttype/)
* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


