---
title: "DifLoadOptions.DifLoadOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor DifLoadOptions. Las opciones"
type: docs
url: /es/net/aspose.cells.loading/difloadoptions/difloadoptions/
---
## DifLoadOptions constructor

Las opciones.

```csharp
public DifLoadOptions()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Loading;
    using System;

    public class DifLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            try
            {
                // Cree una nueva instancia de DifLoadOptions usando el constructor sin parámetros
                DifLoadOptions loadOptions = new DifLoadOptions();

                // Cree un nuevo libro de trabajo con opciones predeterminadas
                Workbook workbook = new Workbook();

                // Acceder a la primera hoja de cálculo
                Worksheet worksheet = workbook.Worksheets[0];

                // Agregue datos de muestra para demostrar que el libro de trabajo funciona
                worksheet.Cells["A1"].PutValue("DifLoadOptions Constructor Demo");
                worksheet.Cells["A2"].PutValue("Created at: " + DateTime.Now.ToString());
                worksheet.Cells["A4"].PutValue("This demonstrates using the parameterless constructor");

                // Guardar el libro de trabajo en formato DIF
                workbook.Save("DifLoadOptionsCtorDemo.dif", SaveFormat.Dif);

                // Ahora cargue el archivo DIF guardado con DifLoadOptions
                DifLoadOptions difOptions = new DifLoadOptions();
                Workbook loadedWorkbook = new Workbook("DifLoadOptionsCtorDemo.dif", difOptions);

                // Guardar los datos cargados en XLSX para verificación
                loadedWorkbook.Save("DifLoadOptionsCtorVerification.xlsx", SaveFormat.Xlsx);

                Console.WriteLine("DifLoadOptions constructor demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing DifLoadOptions constructor demo: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [DifLoadOptions](../)
* namespace [Aspose.Cells.Loading](../../../aspose.cells.loading/)
* assembly [Aspose.Cells](../../../)


