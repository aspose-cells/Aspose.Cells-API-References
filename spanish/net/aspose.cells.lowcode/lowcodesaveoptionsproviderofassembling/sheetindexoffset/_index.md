---
title: "LowCodeSaveOptionsProviderOfAssembling.SheetIndexOffset"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LowCodeSaveOptionsProviderOfAssembling. Desplazamiento del índice de las hojas entre lo que se usa en la ruta del archivo y su valor real SheetIndex"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/sheetindexoffset/
---
## LowCodeSaveOptionsProviderOfAssembling.SheetIndexOffset property

Desplazamiento del índice de la hoja entre lo que se usa en la ruta del archivo y su valor real ([`SheetIndex`](../../splitpartinfo/sheetindex/)).

```csharp
public int SheetIndexOffset { get; set; }
```

### Observaciones

Solo tiene efecto cuando [`UseSheetName`](../usesheetname/) es false.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertySheetIndexOffsetDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con varias hojas
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("SalesData");
            workbook.Worksheets.Add("Inventory");

            // Inicializar el proveedor de opciones de guardado
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "output/Quarter_",
                PathTail = ".xlsx",
                SheetPrefix = "Sheet",
                SheetIndexOffset = 10,
                SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Xlsx }
            };

            // Mostrar el desplazamiento original
            Console.WriteLine($"Original SheetIndexOffset: {provider.SheetIndexOffset}");

            // Guardar con el desplazamiento inicial (las hojas se numerarán 10 y 11)
            workbook.Save("output/with_offset", provider.SaveOptionsTemplate.SaveFormat);

            // Cambiar el desplazamiento y guardar de nuevo
            provider.SheetIndexOffset = 100;
            Console.WriteLine($"Modified SheetIndexOffset: {provider.SheetIndexOffset}");
            
            // Guardar con el nuevo desplazamiento (las hojas se numerarán 100 y 101)
            workbook.Save("output/with_modified_offset", provider.SaveOptionsTemplate.SaveFormat);
        }
    }
}
```

### Ver también

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


