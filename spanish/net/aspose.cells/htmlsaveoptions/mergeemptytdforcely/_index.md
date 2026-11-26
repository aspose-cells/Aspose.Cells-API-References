---
title: "HtmlSaveOptions.MergeEmptyTdForcely"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si se fusiona forzadamente el elemento TD vacío al exportar el archivo a html. El tamaño del archivo html se reducirá significativamente después de establecer el valor en true. El valor predeterminado es false. Si deseas importar el archivo html a excel o exportar líneas de cuadrícula perfectas al guardar el archivo en html, por favor mantén el valor predeterminado."
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/mergeemptytdforcely/
---
## HtmlSaveOptions.MergeEmptyTdForcely property

Indica si se fusiona forzadamente el elemento TD vacío al exportar el archivo a html. El tamaño del archivo html se reducirá significativamente después de establecer el valor en true. El valor predeterminado es false. Si deseas importar el archivo html a excel o exportar líneas de cuadrícula perfectas al guardar el archivo en html, por favor mantén el valor predeterminado.

```csharp
[Obsolete("Use HtmlSaveOptions.MergeEmptyTdType instead.")]
public bool MergeEmptyTdForcely { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyMergeEmptyTdForcelyDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de ejemplo con celdas vacías
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear algunas celdas vacías en la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            // B2 se deja intencionalmente vacío
            
            // Guardar con MergeEmptyTdForcely habilitado
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.MergeEmptyTdForcely = true;
            workbook.Save("output_with_merge.html", options);
            
            // Guardar sin MergeEmptyTdForcely para comparación
            options.MergeEmptyTdForcely = false;
            workbook.Save("output_without_merge.html", options);
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


