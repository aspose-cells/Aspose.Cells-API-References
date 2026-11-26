---
title: "Enum MergeEmptyTdType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.MergeEmptyTdType. Representa el tipo de fusión para un elemento TD vacío al exportar un archivo a HTML"
type: docs
url: /es/net/aspose.cells/mergeemptytdtype/
---
## MergeEmptyTdType enumeration

Representa el tipo de combinación para un elemento TD vacío al exportar un archivo a HTML.

```csharp
public enum MergeEmptyTdType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Default | `0` | Mostrar como MS Excel. |
| None | `1` | Los elementos TD vacíos no se fusionarán al exportar el archivo a html. Esto generará un archivo html significativamente más grande. |
| MergeForcely | `2` | Fusión forzada del elemento TD vacío al exportar el archivo a html. El tamaño del archivo html se reducirá significativamente después de establecer el valor en true. Si desea importar el archivo html a Excel o exportar líneas de cuadrícula perfectas al guardar el archivo en html, mantenga el valor predeterminado. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MergeEmptyTdTypeDemo
    {
        public static void MergeEmptyTdTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Data1");
            worksheet.Cells["B1"].PutValue("Data2");
            worksheet.Cells["C1"].PutValue("Data3");

            // Cree HtmlSaveOptions y establezca la propiedad MergeEmptyTdType
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.MergeEmptyTdType = MergeEmptyTdType.MergeForcely;

            // Guarde el libro de trabajo en formato HTML
            workbook.Save("MergeEmptyTdTypeExample.html", saveOptions);

            Console.WriteLine("HTML file saved with MergeEmptyTdType.MergeForcely option.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


