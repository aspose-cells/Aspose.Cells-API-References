---
title: "Clase LowCodeHtmlSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.LowCode.LowCodeHtmlSaveOptions. Opciones para guardar HTML de forma de bajo código"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodehtmlsaveoptions/
---
## LowCodeHtmlSaveOptions class

Opciones para guardar html de forma low code.

```csharp
public class LowCodeHtmlSaveOptions : LowCodeSaveOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [LowCodeHtmlSaveOptions](lowcodehtmlsaveoptions/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [HtmlOptions](../../aspose.cells.lowcode/lowcodehtmlsaveoptions/htmloptions/) { get; set; } | Las opciones generales para guardar HTML. |
| [OutputFile](../../aspose.cells.lowcode/lowcodesaveoptions/outputfile/) { get; set; } | Obtiene y establece el archivo (con ruta si es necesario) para guardar los datos generados. Al establecer esta propiedad con un valor distinto de null o cadena vacía, [`OutputStream`](../lowcodesaveoptions/outputstream/) será ignorado.(Hereda de [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| [OutputStream](../../aspose.cells.lowcode/lowcodesaveoptions/outputstream/) { get; set; } | Obtiene y establece el Stream para escribir los datos generados. Al establecer esta propiedad con un valor distinto de null, [`OutputFile`](../lowcodesaveoptions/outputfile/) será ignorado.(Hereda de [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| override [SaveFormat](../../aspose.cells.lowcode/lowcodehtmlsaveoptions/saveformat/) { get; set; } | Obtiene y establece el formato de la hoja de cálculo. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassLowCodeHtmlSaveOptionsDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Widget");
            worksheet.Cells["B2"].PutValue(29.99);

            // Crea y configura LowCodeHtmlSaveOptions
            LowCodeHtmlSaveOptions saveOptions = new LowCodeHtmlSaveOptions
            {
                HtmlOptions = new HtmlSaveOptions()
                {
                    ExportWorksheetCSSSeparately = false,
                    ExportImagesAsBase64 = true
                }
            };

            // Guarda el libro de trabajo con las opciones HTML configuradas usando el parámetro de opciones de guardado
            workbook.Save("LowCodeHtmlExport.html", saveOptions.HtmlOptions);

            Console.WriteLine("HTML file saved successfully with low code options.");
        }
    }
}
```

### Ver también

* class [LowCodeSaveOptions](../lowcodesaveoptions/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


