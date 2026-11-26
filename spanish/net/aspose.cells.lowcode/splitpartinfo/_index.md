---
title: "Clase SplitPartInfo"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.LowCode.SplitPartInfo. Representa la información de una entrada/salida para múltiples entradas/salidas, como la página actual que se renderizará al convertir la hoja de cálculo a imagen"
type: docs
url: /es/net/aspose.cells.lowcode/splitpartinfo/
---
## SplitPartInfo class

Representa la información de una entrada/salida para múltiples entradas/salidas, como la página actual que se renderizará al convertir una hoja de cálculo a imagen.

```csharp
public class SplitPartInfo
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [PartIndex](../../aspose.cells.lowcode/splitpartinfo/partindex/) { get; } | Índice de la parte actual en la secuencia (basado en 0). -1 indica que no hay múltiples partes, por lo que el resultado es único. |
| [SheetIndex](../../aspose.cells.lowcode/splitpartinfo/sheetindex/) { get; } | Índice de la hoja donde se encuentra la parte actual. -1 indica que solo hay una hoja. |
| [SheetName](../../aspose.cells.lowcode/splitpartinfo/sheetname/) { get; } | Nombre de la hoja donde se encuentra la parte actual. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassSplitPartInfoDemo
    {
        public static void Run()
        {
            try
            {
                // Crea un libro de trabajo con múltiples hojas para la demostración
                Workbook workbook = new Workbook();
                workbook.Worksheets.Add("Sheet1");
                workbook.Worksheets.Add("Sheet2");
                workbook.Worksheets.Add("Sheet3");

                // Crear LowCodeLoadOptions y LowCodeSplitOptions
                LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
                loadOptions.InputFile = "sample.xlsx";

                LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
                splitOptions.LoadOptions = loadOptions;

                // Crear un proveedor personalizado para demostrar el uso de SplitPartInfo
                splitOptions.SaveOptionsProvider = new CustomSplitOptionsProvider();

                // Procesar la operación de división
                SpreadsheetSplitter.Process(splitOptions);

                Console.WriteLine("Split operation completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CustomSplitOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            // Demostrar el acceso a las propiedades de SplitPartInfo
            Console.WriteLine($"Processing part: Index={partInfo.PartIndex}, SheetIndex={partInfo.SheetIndex}, SheetName={partInfo.SheetName}");

            LowCodeSaveOptions options = new LowCodeSaveOptions();
            options.SaveFormat = SaveFormat.Xlsx;
            options.OutputFile = $"Part_{partInfo.PartIndex}_{partInfo.SheetName}.xlsx";
            return options;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


