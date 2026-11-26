---
title: "LowCodeSaveOptionsProviderOfAssembling.SheetPrefix"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "LowCodeSaveOptionsProviderOfAssembling propiedad. Prefijo para el índice de la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/sheetprefix/
---
## LowCodeSaveOptionsProviderOfAssembling.SheetPrefix property

Prefijo para el índice de la hoja de cálculo.

```csharp
public string SheetPrefix { get; set; }
```

### Observaciones

Si solo hay una hoja de cálculo y [`BuildPathWithSheetAlways`](../buildpathwithsheetalways/) es false, entonces este prefijo y el índice de la hoja (o nombre) no se agregarán a la ruta de archivo resultante.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertySheetPrefixDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            LowCodeSaveOptionsProviderOfAssembling provider = new LowCodeSaveOptionsProviderOfAssembling();
            provider.PathHeader = "output/";
            provider.PathTail = ".xlsx";
            provider.UseSheetName = false;

            Console.WriteLine("Current SheetPrefix: " + provider.SheetPrefix);
            
            provider.SheetPrefix = "Report_";
            Console.WriteLine("New SheetPrefix: " + provider.SheetPrefix);

            for (int sheetIndex = 0; sheetIndex < workbook.Worksheets.Count; sheetIndex++)
            {
                string fileName = $"{provider.PathHeader}{provider.SheetPrefix}{sheetIndex}{provider.PathTail}";
                Console.WriteLine($"Generated file path: {fileName}");
            }

            provider.SheetPrefix = "Data_";
            Console.WriteLine("Updated SheetPrefix: " + provider.SheetPrefix);

            for (int sheetIndex = 0; sheetIndex < workbook.Worksheets.Count; sheetIndex++)
            {
                string fileName = $"{provider.PathHeader}{provider.SheetPrefix}{sheetIndex}{provider.PathTail}";
                Console.WriteLine($"Generated file path: {fileName}");
            }
        }
    }
}
```

### Ver también

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


