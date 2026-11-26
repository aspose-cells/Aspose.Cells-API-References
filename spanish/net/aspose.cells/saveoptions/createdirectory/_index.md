---
title: "SaveOptions.CreateDirectory"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SaveOptions. Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo"
type: docs
url: /es/net/aspose.cells/saveoptions/createdirectory/
---
## SaveOptions.CreateDirectory property

Si es verdadero y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo.

```csharp
public bool CreateDirectory { get; set; }
```

### Observaciones

El valor predeterminado es false.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyCreateDirectoryDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar datos de ejemplo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");

            // Establecer opciones de guardado con CreateDirectory habilitado
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            saveOptions.CreateDirectory = true;

            // Guardar el libro de trabajo en un nuevo directorio (se creará automáticamente)
            string outputPath = "OutputDirectory/example.xls";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("File saved successfully with directory creation.");
        }
    }
}
```

### Ver también

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


