---
title: "Clase SheetSet"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Rendering.SheetSet. Describe un conjunto de hojas"
type: docs
url: /es/net/aspose.cells.rendering/sheetset/
---
## SheetSet class

Describe un conjunto de hojas.

```csharp
public class SheetSet
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [SheetSet](sheetset/#constructor)(params int[]) | Crea un conjunto de hojas basado en índices de hoja exactos. |
| [SheetSet](sheetset/#constructor_1)(params string[]) | Crea un conjunto de hojas basado en nombres de hoja exactos. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| static [Active](../../aspose.cells.rendering/sheetset/active/) { get; } | Obtiene un conjunto con la hoja activa del libro de trabajo. |
| static [All](../../aspose.cells.rendering/sheetset/all/) { get; } | Obtiene un conjunto con todas las hojas del libro de trabajo en su orden original. |
| static [Visible](../../aspose.cells.rendering/sheetset/visible/) { get; } | Obtiene un conjunto con las hojas visibles del libro de trabajo en su orden original. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetSetDemo
    {
        public static void SheetSetExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(456);   

            worksheet = workbook.Worksheets.Add("test1");
            worksheet.Cells["A1"].PutValue("test Data");
            worksheet.Cells["A2"].PutValue(234);
            worksheet.Cells["A3"].PutValue(333);
            worksheet.IsVisible = false;

            worksheet = workbook.Worksheets.Add("test2");
            worksheet.Cells["A1"].PutValue("test Data222");
            worksheet.Cells["A2"].PutValue(234444);
            worksheet.Cells["A3"].PutValue(333555);

            workbook.Worksheets.ActiveSheetIndex = 0;

            // Crea un objeto PdfSaveOptions
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Establece la propiedad SheetSet para incluir solo la hoja activa
            pdfSaveOptions.SheetSet = SheetSet.Active;

            // Guarda el libro de trabajo en un archivo PDF
            workbook.Save("SheetSetExample_ActiveSheet.pdf", pdfSaveOptions);

            // Establezca la propiedad SheetSet para incluir todas las hojas visibles
            pdfSaveOptions.SheetSet = SheetSet.Visible;

            // Guarda el libro de trabajo en un archivo PDF
            workbook.Save("SheetSetExample_VisibleSheets.pdf", pdfSaveOptions);

            // Establezca la propiedad SheetSet para incluir todas las hojas
            pdfSaveOptions.SheetSet = SheetSet.All;

            // Guarda el libro de trabajo en un archivo PDF
            workbook.Save("SheetSetExample_AllSheets.pdf", pdfSaveOptions);

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


