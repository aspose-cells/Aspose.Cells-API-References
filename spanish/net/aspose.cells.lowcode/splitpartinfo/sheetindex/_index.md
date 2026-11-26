---
title: "SplitPartInfo.SheetIndex"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SplitPartInfo. Índice de la hoja donde se encuentra la parte actual. 1 indica que solo hay una hoja"
type: docs
url: /es/net/aspose.cells.lowcode/splitpartinfo/sheetindex/
---
## SplitPartInfo.SheetIndex property

Índice de la hoja donde se encuentra la parte actual. -1 indica que solo hay una hoja.

```csharp
public int SheetIndex { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SplitPartInfoPropertySheetIndexDemo
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
                splitOptions.SaveOptionsProvider = new CustomSheetIndexProvider();

                // Procesar la operación de división
                SpreadsheetSplitter.Process(splitOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CustomSheetIndexProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            // Demostrar la lectura de la propiedad SheetIndex
            Console.WriteLine($"Current part SheetIndex: {partInfo.SheetIndex}");
            Console.WriteLine($"Current part SheetName: {partInfo.SheetName}");
            Console.WriteLine($"Current part PartIndex: {partInfo.PartIndex}");

            LowCodeSaveOptions options = new LowCodeSaveOptions();
            options.SaveFormat = SaveFormat.Xlsx;
            options.OutputFile = $"Sheet_{partInfo.SheetIndex}_{partInfo.SheetName}.xlsx";
            return options;
        }
    }
}
```

### Ver también

* class [SplitPartInfo](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


