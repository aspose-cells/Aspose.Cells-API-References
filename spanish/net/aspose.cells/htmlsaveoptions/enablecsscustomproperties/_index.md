---
title: "HtmlSaveOptions.EnableCssCustomProperties"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Optimiza la salida de html mediante el uso de propiedades personalizadas CSS. Por ejemplo, en el caso de que haya múltiples ocurrencias de una misma imagen base64 con una propiedad personalizada, los datos de la imagen solo necesitan guardarse una vez, lo que mejora el rendimiento del html resultante. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/enablecsscustomproperties/
---
## HtmlSaveOptions.EnableCssCustomProperties property

Optimiza la salida de html usando propiedades personalizadas de CSS. Por ejemplo, en el caso de que haya múltiples ocurrencias de una misma imagen base64, con una propiedad personalizada los datos de la imagen solo necesitan guardarse una vez, lo que mejora el rendimiento del html resultante. El valor predeterminado es false.

```csharp
public bool EnableCssCustomProperties { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class HtmlSaveOptionsPropertyEnableCssCustomPropertiesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra con formato
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["A1"].GetStyle().Font.IsBold = true;
            worksheet.Cells["A1"].GetStyle().Font.Color = System.Drawing.Color.Red;

            // Agregar una imagen que se repetirá en varias celdas
            int imgIndex = worksheet.Pictures.Add(1, 1, "logo.png");
            Picture pic = worksheet.Pictures[imgIndex];
            pic.Move(1, 1); // Using Move instead of LeftOffset/TopOffset
            pic.Width = 100;
            pic.Height = 100;

            // Copiar la imagen a otra ubicación
            worksheet.Cells["D5"].PutValue("Same image reference:");
            int imgIndex2 = worksheet.Pictures.Add(5, 3, "logo.png");
            Picture pic2 = worksheet.Pictures[imgIndex2];
            pic2.Move(5, 3); // Using Move instead of LeftOffset/TopOffset
            pic2.Width = 100;
            pic2.Height = 100;

            // Crear instancia de HtmlSaveOptions
            HtmlSaveOptions htmlOptions = new HtmlSaveOptions();

            // Mostrar el valor actual
            Console.WriteLine("Current EnableCssCustomProperties value: " + htmlOptions.EnableCssCustomProperties);

            // Establecer en verdadero para optimizar la salida CSS
            htmlOptions.EnableCssCustomProperties = true;

            // Guardar con optimización CSS
            workbook.Save("HtmlWithCssCustomProperties.html", htmlOptions);

            // Establecer en falso para comparación
            htmlOptions.EnableCssCustomProperties = false;
            workbook.Save("HtmlWithoutCssCustomProperties.html", htmlOptions);

            Console.WriteLine("Files saved with and without CSS custom properties optimization.");
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


