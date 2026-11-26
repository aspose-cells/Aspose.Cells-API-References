---
title: "PdfSaveOptions.Producer"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PdfSaveOptions. Obtiene y establece el productor del documento pdf generado"
type: docs
url: /es/net/aspose.cells/pdfsaveoptions/producer/
---
## PdfSaveOptions.Producer property

Obtiene y establece el productor del documento pdf generado.

```csharp
public string Producer { get; set; }
```

### Observaciones

Si el valor es nulo, o no se establece una LICENSE válida, se utilizará la cadena Aspose.Cells vVERSION.

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyProducerDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceda a la primera hoja de cálculo y agregue datos de ejemplo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("PDF Producer Property Demo");

            // Crea opciones de guardado PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Establecer la propiedad Producer
            pdfSaveOptions.Producer = "Aspose.Cells for .NET";
            
            // Guardar en flujo de memoria
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, pdfSaveOptions);
                
                // Verificar que la propiedad Producer se haya establecido
                stream.Position = 0;
                using (StreamReader reader = new StreamReader(stream))
                {
                    string content = reader.ReadToEnd();
                    Console.WriteLine(content.Contains("/Producer (Aspose.Cells for .NET)") 
                        ? "Producer property set successfully" 
                        : "Failed to set Producer property");
                }
            }
        }
    }
}
```

### Ver también

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


