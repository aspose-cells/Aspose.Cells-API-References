---
title: "FileFormatInfo.LoadFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FileFormatInfo. Obtiene el formato de carga detectado"
type: docs
url: /es/net/aspose.cells/fileformatinfo/loadformat/
---
## FileFormatInfo.LoadFormat property

Obtiene el formato de carga detectado.

```csharp
public LoadFormat LoadFormat { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatInfoPropertyLoadFormatDemo
    {
        public static void Run()
        {
            // La ruta al directorio de documentos.
            string filePath = "data/";
            
            // Detectar formato de archivo
            string fileName = "SAMPLE_XLS_ISSUE.XLS";
            var fileFormatInfo = FileFormatUtil.DetectFileFormat(filePath + fileName);
            Console.WriteLine("Detected LoadFormat: " + fileFormatInfo.LoadFormat);

            // Cargar archivo con el formato correcto
            LoadOptions loadOptions = new LoadOptions(LoadFormat.MHtml);
            var workbook = new Workbook(filePath + fileName, loadOptions);
            
            // Procesar el libro de trabajo
            workbook.Worksheets[0].AutoFitColumns();
            workbook.Save(filePath + "output.xlsx");
        }
    }
}
```

### Ver también

* enum [LoadFormat](../../loadformat/)
* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


