---
title: "LowCodeSaveOptionsProviderOfAssembling.UseSheetName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "LowCodeSaveOptionsProviderOfAssembling property. Indica si construye la ruta del archivo con el nombre de la hoja en lugar del índice de la hoja. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/usesheetname/
---
## LowCodeSaveOptionsProviderOfAssembling.UseSheetName property

Indica si se construye la ruta del archivo con el nombre de la hoja en lugar del índice de la hoja. El valor predeterminado es false.

```csharp
public bool UseSheetName { get; set; }
```

### Observaciones

El nombre de la hoja nunca se volverá a generar automáticamente. Por lo tanto, cuando se establezca en true, asegúrese de que no haya ningún nombre de hoja especial que pueda causar una ruta de archivo o nombre inválido.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertyUseSheetNameDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con una hoja de cálculo nombrada
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "MonthlyReport";
            
            // Agrega datos de ejemplo para la demostración de división
            for(int i = 0; i < 15; i++)
            {
                worksheet.Cells[$"A{i+1}"].PutValue($"Record {i+1}");
            }

            // Crea y configura el proveedor
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "split_files/",
                PathTail = ".xlsx",
                SheetPrefix = "Sheet_",
                SplitPartPrefix = "Part_",
                SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Xlsx }
            };

            // Demuestra UseSheetName=false (predeterminado)
            Console.WriteLine($"Default UseSheetName: {provider.UseSheetName}");
            workbook.Save("output_default", provider.SaveOptionsTemplate.SaveFormat);

            // Cambia la propiedad y demuestra el nuevo comportamiento
            provider.UseSheetName = true;
            Console.WriteLine($"\nModified UseSheetName: {provider.UseSheetName}");
            workbook.Save("output_modified", provider.SaveOptionsTemplate.SaveFormat);

            Console.WriteLine("Check 'split_files' directory for output files with different naming schemes");
        }
    }
}
```

### Ver también

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


