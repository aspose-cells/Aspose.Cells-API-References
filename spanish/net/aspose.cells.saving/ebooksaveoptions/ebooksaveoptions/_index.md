---
title: "EbookSaveOptions.EbookSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor de EbookSaveOptions. Crea opciones para guardar un archivo ebook"
type: docs
url: /es/net/aspose.cells.saving/ebooksaveoptions/ebooksaveoptions/
---
## EbookSaveOptions() {#constructor}

Crea opciones para guardar el archivo ebook.

```csharp
public EbookSaveOptions()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class EbookSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar contenido de ejemplo
            worksheet.Cells["A1"].PutValue("Ebook Test");
            worksheet.Cells["A2"].PutValue("This is a test for EbookSaveOptions");
            
            // Crear EbookSaveOptions usando el constructor
            EbookSaveOptions saveOptions = new EbookSaveOptions();
            
            // Guarde el libro de trabajo con EbookSaveOptions (se guarda automáticamente como EPUB)
            workbook.Save("output.epub", saveOptions);
            
            Console.WriteLine("Ebook saved successfully with EbookSaveOptions constructor.");
        }
    }
}
```

### Ver también

* class [EbookSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)

---

## EbookSaveOptions(SaveFormat) {#constructor_1}

Crea opciones para guardar el archivo ebook.

```csharp
public EbookSaveOptions(SaveFormat saveFormat)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| saveFormat | SaveFormat | El formato de archivo. Debe ser Epub o Azw3. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class EbookSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Sample Ebook Content");
            
            try
            {
                // Llamar al método #ctor con el parámetro SaveFormat
                EbookSaveOptions saveOptions = new EbookSaveOptions(SaveFormat.Epub);
                
                // Establezca propiedades adicionales si es necesario
                saveOptions.Encoding = System.Text.Encoding.UTF8;
                
                Console.WriteLine("EbookSaveOptions constructor executed successfully with SaveFormat.Epub");
                
                // Guardar el libro de trabajo con las opciones creadas
                workbook.Save("EbookSaveOptionsDemo.epub", saveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing EbookSaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [EbookSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


