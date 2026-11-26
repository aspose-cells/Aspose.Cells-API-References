---
title: "Clase AbstractLowCodeSaveOptionsProvider"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.LowCode.AbstractLowCodeSaveOptionsProvider. Implementación para proporcionar múltiples opciones de guardado para procesos que requieren múltiples salidas. Por ejemplo, la función SpreadsheetSplitter requiere múltiples destinos para guardar los archivos divididos."
type: docs
url: /es/net/aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/
---
## AbstractLowCodeSaveOptionsProvider class

Implementación para proporcionar múltiples opciones de guardado para procesos que requieren múltiples salidas. Por ejemplo, la función [`SpreadsheetSplitter`](../spreadsheetsplitter/) requiere múltiples destinos para guardar los archivos divididos.

```csharp
public abstract class AbstractLowCodeSaveOptionsProvider
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/)(LowCodeSaveOptions) | Libera recursos después de procesar la parte dividida actual. |
| abstract [GetSaveOptions](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/getsaveoptions/)(SplitPartInfo) | Obtiene las opciones de guardado de las que se extraen la configuración de salida para la parte dividida actual. Devolver null indica omitir la parte dada. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassAbstractLowCodeSaveOptionsProviderDemo
    {
        public static void Run()
        {
            // Crea un proveedor personalizado extendiendo AbstractLowCodeSaveOptionsProvider
            var customProvider = new CustomSaveOptionsProvider();

            // Crea un libro de trabajo y una hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Poblar algunos datos
            worksheet.Cells["A1"].PutValue("Test Data");
            
            // Crear información de la parte dividida - en uso real, esto provendría de la API
            // Dado que no podemos construirlo directamente, simplemente pasaremos null para la demostración
            SplitPartInfo splitPartInfo = null;
            
            // Obtener opciones de guardado del proveedor
            LowCodeSaveOptions saveOptions = customProvider.GetSaveOptions(splitPartInfo);
            
            // Configurar opciones de guardado (ejemplo)
            saveOptions.SaveFormat = SaveFormat.Xlsx;
            
            // Demostrar la finalización del proceso
            customProvider.Finish(saveOptions);
            
            // Guardar el libro de trabajo (no está directamente relacionado con el proveedor, solo para la demostración)
            workbook.Save("LowCodeSaveOptionsDemo.xlsx");
        }
    }

    // Implementación personalizada de AbstractLowCodeSaveOptionsProvider
    public class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
        {
            // Crear y devolver opciones de guardado personalizadas basadas en la información de la parte
            return new LowCodeSaveOptions()
            {
                SaveFormat = SaveFormat.Xlsx
                // Eliminado CachedFileFolder ya que no existe en LowCodeSaveOptions
            };
        }

        public override void Finish(LowCodeSaveOptions part)
        {
            // Lógica de limpieza o finalización aquí
            Console.WriteLine("Save operation completed for part");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


