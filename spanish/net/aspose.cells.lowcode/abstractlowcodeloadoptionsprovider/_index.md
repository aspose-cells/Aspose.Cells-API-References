---
title: "Clase AbstractLowCodeLoadOptionsProvider"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.LowCode.AbstractLowCodeLoadOptionsProvider. Implementación para proporcionar múltiples opciones de carga para procesos que utilizan múltiples entradas, como archivos de plantilla"
type: docs
url: /es/net/aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/
---
## AbstractLowCodeLoadOptionsProvider class

Implementación para proporcionar múltiples opciones de carga para procesos que utilizan múltiples entradas (como archivos de plantilla).

```csharp
public abstract class AbstractLowCodeLoadOptionsProvider
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| abstract [Current](../../aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/current/) { get; } | Obtiene las opciones de carga desde las cuales cargar los datos de la parte procesada actualmente. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/finish/)(LowCodeLoadOptions) | Libera recursos después de procesar la parte actual de la entrada. |
| abstract [MoveNext](../../aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/movenext/)() | Comprueba si hay más entrada. |

### Observaciones

Por ejemplo, la característica [`SpreadsheetMerger`](../spreadsheetmerger/) requiere varios archivos de plantilla para combinar.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassAbstractLowCodeLoadOptionsProviderDemo
    {
        public static void Run()
        {
            // Crea una implementación personalizada de AbstractLowCodeLoadOptionsProvider
            var provider = new CustomLoadOptionsProvider();

            // Procesa múltiples entradas usando el proveedor
            while (provider.MoveNext())
            {
                // Obtén las opciones de carga actuales
                LowCodeLoadOptions currentOptions = provider.Current;
                Console.WriteLine($"Processing with load options: {currentOptions}");

                // Crea un libro de trabajo con las opciones actuales
                Workbook workbook = new Workbook(FileFormatType.Xlsx);
                Worksheet worksheet = workbook.Worksheets[0];

                // Demuestra el uso con el libro de trabajo
                worksheet.Cells["A1"].PutValue("Processed with custom provider");
                
                // Finaliza el procesamiento de esta parte
                provider.Finish(currentOptions);
            }
        }

        private class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
        {
            private int currentIndex = 0;
            private readonly LowCodeLoadOptions[] optionsList = new LowCodeLoadOptions[]
            {
                new LowCodeLoadOptions(),
                new LowCodeLoadOptions { InputFile = "protected.xlsx" }, // Password would be handled separately
                new LowCodeLoadOptions() // MemorySetting would be handled separately
            };

            public override LowCodeLoadOptions Current => optionsList[currentIndex];

            public override bool MoveNext()
            {
                if (currentIndex < optionsList.Length - 1)
                {
                    currentIndex++;
                    return true;
                }
                return false;
            }

            public override void Finish(LowCodeLoadOptions part)
            {
                // Lógica de limpieza o finalización para cada parte
                Console.WriteLine($"Finished processing part {currentIndex}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


