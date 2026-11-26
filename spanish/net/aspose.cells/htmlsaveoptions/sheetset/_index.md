---
title: "HtmlSaveOptions.SheetSet"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Obtiene o establece las hojas a renderizar. El valor predeterminado es todas las hojas visibles en el libro de trabajo Visible"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/sheetset/
---
## HtmlSaveOptions.SheetSet property

Obtiene o establece las hojas a renderizar. El valor predeterminado es todas las hojas visibles en el libro de trabajo: [`Visible`](../../../aspose.cells.rendering/sheetset/visible/).

```csharp
public SheetSet SheetSet { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class HtmlSaveOptionsPropertySheetSetDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con múltiples hojas de cálculo
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // Ocultar una hoja para la demostración
            workbook.Worksheets[1].IsVisible = false;

            // Establecer algunos datos de ejemplo en cada hoja
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Worksheet sheet = workbook.Worksheets[i];
                sheet.Cells["A1"].PutValue($"Data from {sheet.Name}");
            }

            // Crear instancia de HtmlSaveOptions
            HtmlSaveOptions options = new HtmlSaveOptions();

            // Mostrar el valor actual de SheetSet (el predeterminado es null, lo que significa todas las hojas visibles)
            Console.WriteLine("Current SheetSet value: " + (options.SheetSet == null ? "All visible sheets" : "Custom set"));

            // Establecer SheetSet para incluir solo hojas específicas (por índice)
            options.SheetSet = new SheetSet(new int[] { 0, 2 });

            // Guardar como HTML - solo se incluirán las hojas especificadas
            workbook.Save("HtmlWithCustomSheetSet.html", options);

            // Cambiar SheetSet a solo hojas visibles
            options.SheetSet = SheetSet.Visible;
            workbook.Save("HtmlWithVisibleSheets.html", options);

            // Cambiar SheetSet a solo la hoja activa
            workbook.Worksheets[2].IsSelected = true; // Activate the sheet by selecting it
            options.SheetSet = SheetSet.Active;
            workbook.Save("HtmlWithActiveSheet.html", options);
        }
    }
}
```

### Ver también

* class [SheetSet](../../../aspose.cells.rendering/sheetset/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


