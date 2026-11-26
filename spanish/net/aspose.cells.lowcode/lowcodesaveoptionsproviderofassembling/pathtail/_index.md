---
title: "LowCodeSaveOptionsProviderOfAssembling.PathTail"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "LowCodeSaveOptionsProviderOfAssembling property. Parte final después de los números de secuencia de la ruta del archivo. Debe incluir la extensión del nombre de archivo"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/pathtail/
---
## LowCodeSaveOptionsProviderOfAssembling.PathTail property

Parte final (después de los números de secuencia) de la ruta del archivo. Debe incluir la extensión del nombre del archivo.

```csharp
public string PathTail { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertyPathTailDemo
    {
        public static void Run()
        {
            // Crear libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 25; i++)
            {
                worksheet.Cells[i, 0].Value = $"Record {i + 1}";
            }

            // Inicializar el proveedor de opciones de guardado
            var optionsProvider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "SalesReports/Q3",
                PathTail = ".xlsx",
                UseSheetName = true,
                SaveOptionsTemplate = new LowCodeSaveOptions
                {
                    SaveFormat = SaveFormat.Xlsx
                }
            };

            Console.WriteLine($"Original file extension: {optionsProvider.PathTail}");

            // Primera guardada con la extensión predeterminada
            workbook.Save("output_original", optionsProvider.SaveOptionsTemplate.SaveFormat);

            // Modifica la parte final de la ruta para la salida CSV
            optionsProvider.PathTail = "_split.csv";
            optionsProvider.SaveOptionsTemplate.SaveFormat = SaveFormat.Csv;
            Console.WriteLine($"Modified file extension: {optionsProvider.PathTail}");

            // Segunda guardada con la nueva extensión
            workbook.Save("output_modified", optionsProvider.SaveOptionsTemplate.SaveFormat);

            Console.WriteLine("Check output directories for generated file formats");
        }
    }
}
```

### Ver también

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


