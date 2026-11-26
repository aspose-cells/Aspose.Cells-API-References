---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.SheetNamePrefix"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LowCodeSaveOptionsProviderOfPlaceHolders. Prefijo para el índice de la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetnameprefix/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.SheetNamePrefix property

Prefijo para el índice de la hoja de cálculo.

```csharp
public string SheetNamePrefix { get; set; }
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

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySheetNamePrefixDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con dos hojas de cálculo
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Name = "SalesData";
            workbook.Worksheets.Add("FinancialReport");

            // Inicializar el proveedor con una plantilla de ruta que contiene el marcador de posición de hoja
            string pathTemplate = "output_{sheet}.xlsx";
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders(pathTemplate);

            // Mostrar el valor inicial de SheetNamePrefix (vacío por defecto)
            Console.WriteLine("Initial SheetNamePrefix: " + provider.SheetNamePrefix);

            // Establecer un nuevo prefijo y asegurar que la generación de rutas incluya la información de la hoja
            provider.SheetNamePrefix = "Q4_";
            provider.BuildPathWithSheetAlways = true;

            // Configurar las opciones de guardado con el formato correcto
            provider.SaveOptionsTemplate = new LowCodeSaveOptions
            {
                SaveFormat = SaveFormat.Xlsx // Set the correct save format
            };

            // Guardar el libro de trabajo usando el proveedor - genera "output_Q4_SalesData.xlsx" y "output_Q4_FinancialReport.xlsx"
            workbook.Save("result_directory", SaveFormat.Xlsx); // Pass correct SaveFormat
        }
    }
}
```

### Ver también

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


