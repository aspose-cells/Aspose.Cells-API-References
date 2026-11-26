---
title: "HtmlSaveOptions.IsBorderCollapsed"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si los bordes de la tabla están colapsados. El valor predeterminado es true"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/isbordercollapsed/
---
## HtmlSaveOptions.IsBorderCollapsed property

Indica si los bordes de la tabla están colapsados. El valor predeterminado es true.

```csharp
public bool IsBorderCollapsed { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using System.Threading;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsBorderCollapsedDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra y bordes
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["B2"].PutValue("With Borders");
            worksheet.Cells["B2"].SetStyle(style);

            // Establecer la cultura para la demostración
            var culture = new System.Globalization.CultureInfo("de-DE");
            Thread.CurrentThread.CurrentCulture = culture;
            Thread.CurrentThread.CurrentUICulture = culture;
            workbook.Settings.CultureInfo = culture;

            // Crear opciones de guardado HTML y establecer IsBorderCollapsed
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            saveOptions.IsBorderCollapsed = false;

            // Guardar el libro de trabajo con opciones HTML
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "HtmlWithBorders.html");
            workbook.Save(outputPath, saveOptions);

            Console.WriteLine("File saved with collapsed borders: " + outputPath);
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


