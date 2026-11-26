---
title: "SplitPartInfo.SheetName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SplitPartInfo. Nombre de la hoja donde se encuentra la parte actual"
type: docs
url: /es/net/aspose.cells.lowcode/splitpartinfo/sheetname/
---
## SplitPartInfo.SheetName property

Nombre de la hoja donde se encuentra la parte actual.

```csharp
public string SheetName { get; }
```

### Observaciones

Puede ser nulo en algunas situaciones, como al renderizar todo el libro de trabajo a una imagen TIFF.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using AsposeCellsExamples.AbstractLowCodeSaveOptionsProviderMethodFinishWithLowCodeSaveOptionsDemo;
    using System;
    using System.Reflection;

    public class SplitPartInfoPropertySheetNameDemo
    {
        public static void Run()
        {
            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            loadOptions.InputFile = "split.xlsx";

            // Crea una instancia concreta del proveedor
            var provider = new CustomLowCodeSaveOptionsProvider();

            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
            splitOptions.SaveOptionsProvider = provider;
            splitOptions.LoadOptions = loadOptions;

            SpreadsheetSplitter.Process(splitOptions);
        }
    }

    // Implementación concreta de AbstractLowCodeSaveOptionsProvider
    public class CustomLowCodeSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override void Finish(LowCodeSaveOptions part)
        {
            base.Finish(part);
        }
        // Implementa el método abstracto requerido
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            LowCodeSaveOptions result = new LowCodeSaveOptions();
            result.SaveFormat = SaveFormat.Xlsx;
            result.OutputFile = partInfo.SheetName + "_split.xlsx";
            Console.WriteLine(result.OutputFile);
            return result;
        }
    }
}
```

### Ver también

* class [SplitPartInfo](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


