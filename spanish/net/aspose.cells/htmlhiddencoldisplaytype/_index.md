---
title: "Enum HtmlHiddenColDisplayType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.HtmlHiddenColDisplayType. Representa dos tipos de visualización de las columnas ocultas en html"
type: docs
url: /es/net/aspose.cells/htmlhiddencoldisplaytype/
---
## HtmlHiddenColDisplayType enumeration

Representa dos tipos de visualización de columnas ocultas en HTML.

```csharp
public enum HtmlHiddenColDisplayType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Hidden | `0` | Oculta las columnas ocultas en la página html. |
| Remove | `1` | Elimina las columnas ocultas en la página html. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlHiddenColDisplayTypeDemo
    {
        public static void HtmlHiddenColDisplayTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Doe");

            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(35);

            // Oculta la segunda columna
            worksheet.Cells.HideColumn(1);

            // Crea HtmlSaveOptions y establece HiddenColDisplayType
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.HiddenColDisplayType = HtmlHiddenColDisplayType.Remove;

            // Guarde el libro de trabajo en formato HTML
            workbook.Save("HtmlHiddenColDisplayTypeExample.html", saveOptions);

            Console.WriteLine("Workbook saved as HTML with hidden columns removed.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


