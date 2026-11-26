---
title: "SaveOptions.CachedFileFolder"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SaveOptions. La carpeta para archivos temporales que pueden usarse como caché de datos"
type: docs
url: /es/net/aspose.cells/saveoptions/cachedfilefolder/
---
## SaveOptions.CachedFileFolder property

La carpeta para archivos temporales que pueden usarse como caché de datos.

```csharp
public string CachedFileFolder { get; set; }
```

### Observaciones

Si no se ha especificado la carpeta, el valor predeterminado es [`GetCacheFolder`](../../cellshelper/getcachefolder/). Si su valor predeterminado es null o está vacío, o se ha especificado como null o vacío, entonces no se utilizará ningún archivo de caché al guardar el libro de trabajo.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyCachedFileFolderDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test cached file folder");

            // Establecer opciones de guardado con carpeta de archivos en caché
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();
            saveOptions.CachedFileFolder = "TempCache"; // Specify cache folder

            // Guarda el libro de trabajo
            workbook.Save("output.xml", saveOptions);
            
            Console.WriteLine("File saved with cached file folder option.");
        }
    }
}
```

### Ver también

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


