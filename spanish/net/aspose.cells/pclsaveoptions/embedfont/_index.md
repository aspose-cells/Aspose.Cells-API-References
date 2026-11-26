---
title: "PclSaveOptions.EmbedFont"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PclSaveOptions. Indica si se debe incrustar la fuente en el archivo Pcl de salida"
type: docs
url: /es/net/aspose.cells/pclsaveoptions/embedfont/
---
## PclSaveOptions.EmbedFont property

Indica si se debe incrustar la fuente en el archivo Pcl de salida.

```csharp
public bool EmbedFont { get; set; }
```

### Observaciones

El valor predeterminado es true.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PclSaveOptionsPropertyEmbedFontDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo y agregue algunos datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Demonstrating EmbedFont property");
            sheet.Cells["A2"].PutValue(DateTime.Now);

            try
            {
                // Crear opciones de guardado PCL
                PclSaveOptions pclOptions = new PclSaveOptions();

                // Lee y muestra el valor actual de la propiedad EmbedFont
                Console.WriteLine("Current EmbedFont value: " + pclOptions.EmbedFont);

                // (Opcional) Si la propiedad es escribible podrías establecerla, pero solo la leemos aquí
                // pclOptions.EmbedFont = true;

                // Guarda el libro de trabajo como un archivo PCL usando las opciones
                workbook.Save("EmbedFontDemo.pcl", pclOptions);

                Console.WriteLine("Workbook saved successfully with EmbedFont demonstration.");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### Ver también

* class [PclSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


