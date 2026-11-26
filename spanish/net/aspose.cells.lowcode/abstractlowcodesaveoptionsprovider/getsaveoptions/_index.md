---
title: "AbstractLowCodeSaveOptionsProvider.GetSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método AbstractLowCodeSaveOptionsProvider. Obtiene las opciones de guardado desde las cuales obtener la configuración de salida para la parte actualmente dividida. Devolver null indica omitir la parte dada."
type: docs
url: /es/net/aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/getsaveoptions/
---
## AbstractLowCodeSaveOptionsProvider.GetSaveOptions method

Obtiene las opciones de guardado de las que se extraen la configuración de salida para la parte dividida actual. Devolver null indica omitir la parte dada.

```csharp
public abstract LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using AsposeCellsExamples.AbstractLowCodeSaveOptionsProviderMethodFinishWithLowCodeSaveOptionsDemo;
    using System;

    public class AbstractLowCodeSaveOptionsProviderMethodGetSaveOptionsWithSplitPartInfoDemo
    {
        public static void Run()
        {
            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            loadOptions.InputFile = "split.xlsx";

            // Crea una instancia concreta del proveedor
            var provider = new CustomSaveOptionsProvider();

            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
            splitOptions.SaveOptionsProvider = provider;
            splitOptions.LoadOptions = loadOptions;

            SpreadsheetSplitter.Process(splitOptions);
        }
    }

    // Implementación personalizada de AbstractLowCodeSaveOptionsProvider
    public class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            // Crea opciones de guardado personalizadas basadas en la información de la parte
            LowCodeSaveOptions result = new LowCodeSaveOptions();
            result.SaveFormat = SaveFormat.Xlsx;
            result.OutputFile = $"Part_{partInfo.PartIndex}_Sheet_{partInfo.SheetName}.xlsx";
            Console.WriteLine(result.OutputFile);
            return result;

        }
    }
}
```

### Ver también

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SplitPartInfo](../../splitpartinfo/)
* class [AbstractLowCodeSaveOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


