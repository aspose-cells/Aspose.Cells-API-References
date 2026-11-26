---
title: "HtmlSaveOptions.ExportArea"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Obtiene o establece el CellArea que se exporta de la hoja de cálculo activa actual. Si establece este atributo, el área de impresión de la hoja activa se omitirá. Solo el área especificada se exportará al guardar el archivo en HTML."
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/exportarea/
---
## HtmlSaveOptions.ExportArea property

Obtiene o establece el CellArea de exportación de la hoja de cálculo activa actual. Si establece este atributo, el área de impresión de la hoja activa se omitirá. Solo el área especificada se exportará al guardar el archivo en html.

```csharp
public CellArea ExportArea { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportAreaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Poblar algunos datos en la hoja de cálculo
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Cell {i},{j}");
                }
            }

            // Establecer opciones de guardado HTML con área de exportación
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportArea = CellArea.CreateCellArea("B2", "D5");

            // Guardar el libro de trabajo con el área de exportación especificada
            workbook.Save("output.html", options);
        }
    }
}
```

### Ver también

* struct [CellArea](../../cellarea/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


