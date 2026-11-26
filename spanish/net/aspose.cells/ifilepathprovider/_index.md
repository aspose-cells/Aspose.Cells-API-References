---
title: "Interfaz IFilePathProvider"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Interfaz Aspose.Cells.IFilePathProvider. Representa el proveedor de ruta de archivo exportado"
type: docs
url: /es/net/aspose.cells/ifilepathprovider/
---
## IFilePathProvider interface

Representa el proveedor de ruta de archivo exportado.

```csharp
public interface IFilePathProvider
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| [GetFullName](../../aspose.cells/ifilepathprovider/getfullname/)(string) | Obtiene la ruta completa del archivo por nombre de hoja de cálculo al exportar la hoja de cálculo a HTML por separado. Así, las referencias entre las hojas de cálculo pueden exportarse correctamente. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IFilePathProviderDemo : IFilePathProvider
    {
        // Implementando el método GetFullName de la interfaz IFilePathProvider
        public string GetFullName(string sheetName)
        {
            // Para demostración, devuelve una ruta de archivo simple basada en el nombre de la hoja
            return $"{sheetName}.html";
        }

        public static void IFilePathProviderExample()
        {
            // Crear un nuevo libro de trabajo y agregar algunos datos
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // Crear HtmlSaveOptions y establecer el FilePathProvider
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.FilePathProvider = new IFilePathProviderDemo();

            // Guarde el libro de trabajo en formato HTML
            workbook.Save("IFilePathProviderExample.html", saveOptions);

            Console.WriteLine("Workbook saved to HTML with custom file paths.");
        }
    }


}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


