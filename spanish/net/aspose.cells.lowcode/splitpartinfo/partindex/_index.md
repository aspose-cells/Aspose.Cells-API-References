---
title: "SplitPartInfo.PartIndex"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SplitPartInfo. Índice de la parte actual en una secuencia basada en cero. 1 significa que no hay múltiples partes, por lo que el resultado es único"
type: docs
url: /es/net/aspose.cells.lowcode/splitpartinfo/partindex/
---
## SplitPartInfo.PartIndex property

Índice de la parte actual en la secuencia (basado en 0). -1 indica que no hay múltiples partes, por lo que el resultado es único.

```csharp
public int PartIndex { get; }
```

### Observaciones

Si se necesitan procesar varias hojas y cada hoja se procesa (divide) por separado, el índice de parte siempre comienza en 0 para cada hoja. Por ejemplo, al convertir un libro de trabajo a imágenes, representa el índice de página de salida de la hoja que se está procesando actualmente. Y -1 indica que solo hay una página para la hoja actual.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SplitPartInfoPropertyPartIndexDemo
    {
        public static void Run()
        {
            try
            {
                // Crear un libro de trabajo con varias hojas
                Workbook workbook = new Workbook();
                workbook.Worksheets.Add("Sheet1");
                workbook.Worksheets.Add("Sheet2");
                workbook.Worksheets.Add("Sheet3");

                // Guardar el libro de trabajo para usarlo con la operación de división
                workbook.Save("sample.xlsx");

                // Crear opciones de carga
                LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
                loadOptions.InputFile = "sample.xlsx";

                // Crear opciones de división con un proveedor personalizado
                LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
                splitOptions.LoadOptions = loadOptions;
                splitOptions.SaveOptionsProvider = new CustomPartIndexProvider();

                // Procesar la operación de división
                SpreadsheetSplitter.Process(splitOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CustomPartIndexProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            // Demostrar la lectura de la propiedad PartIndex
            Console.WriteLine($"Current part PartIndex: {partInfo.PartIndex}");
            Console.WriteLine($"Current part SheetIndex: {partInfo.SheetIndex}");
            Console.WriteLine($"Current part SheetName: {partInfo.SheetName}");

            LowCodeSaveOptions options = new LowCodeSaveOptions();
            options.SaveFormat = SaveFormat.Xlsx;
            options.OutputFile = $"Part_{partInfo.PartIndex}_{partInfo.SheetName}.xlsx";
            return options;
        }
    }
}
```

### Ver también

* class [SplitPartInfo](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


