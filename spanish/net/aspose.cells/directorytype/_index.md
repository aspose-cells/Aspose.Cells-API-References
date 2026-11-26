---
title: "Enumeración DirectoryType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.DirectoryType enum. Representa el tipo de directorio del nombre de archivo"
type: docs
url: /es/net/aspose.cells/directorytype/
---
## DirectoryType enumeration

Representa el tipo de directorio del nombre de archivo.

```csharp
public enum DirectoryType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Volume | `0` | Representa una letra de unidad MS-DOS. Va seguida por la letra de unidad. O nombres de archivo UNC, como \\\\server\\share\\myfile.xls |
| SameVolume | `1` | Indica que el libro de origen está en la misma unidad que el libro dependiente (se omite la letra de unidad) |
| DownDirectory | `2` | Indica que el libro de origen está en un subdirectorio del directorio actual. |
| UpDirectory | `3` | Indica que el libro de origen está en el directorio padre del directorio actual. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DirectoryTypeDemo
    {
        public static void DirectoryTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(200);
            worksheet.Cells["A4"].PutValue(300);

            // Agregar un enlace externo al libro
            string externalFileName = "externalWorkbook.xlsx";
            string[] sheetNames = { "Sheet1" };

            // Agregar enlace externo con DirectoryType.Volume
            int linkIndex = workbook.Worksheets.ExternalLinks.Add(DirectoryType.Volume, externalFileName, sheetNames);

            // Recuperar el enlace externo agregado
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[linkIndex];

            // Mostrar los detalles del enlace externo
            Console.WriteLine("External Link Details:");
            Console.WriteLine("File Name: " + externalLink.DataSource);

            // Guarda el libro de trabajo
            workbook.Save("DirectoryTypeExample.xlsx");
            workbook.Save("DirectoryTypeExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


