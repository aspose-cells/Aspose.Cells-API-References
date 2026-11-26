---
title: "LowCodeSaveOptionsProviderOfAssembling.BuildPathWithSplitPartAlways"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "LowCodeSaveOptionsProviderOfAssembling propiedad. Si se debe agregar siempre el índice de la parte dividida a la ruta del archivo. El valor predeterminado es false, lo que significa que cuando solo hay una parte dividida, el índice de la parte dividida y el prefijo correspondiente no se agregarán a la ruta del archivo"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/buildpathwithsplitpartalways/
---
## LowCodeSaveOptionsProviderOfAssembling.BuildPathWithSplitPartAlways property

Indica si se agrega siempre el índice de la parte dividida a la ruta del archivo. El valor predeterminado es false, es decir, cuando solo hay una parte dividida, el índice de la parte dividida y el prefijo correspondiente no se agregarán a la ruta del archivo.

```csharp
public bool BuildPathWithSplitPartAlways { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertyBuildPathWithSplitPartAlwaysDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            for (int i = 0; i < 20; i++)
            {
                worksheet.Cells[i, 0].Value = "Data Row " + (i + 1);
            }

            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "SplitData/",
                PathTail = ".xlsx",
                SplitPartPrefix = "Part_",
                SaveOptionsTemplate = new LowCodeSaveOptions()
            };

            Console.WriteLine("Initial BuildPathWithSplitPartAlways: " + provider.BuildPathWithSplitPartAlways);
            workbook.Save("Output1", provider.SaveOptionsTemplate.SaveFormat);

            provider.BuildPathWithSplitPartAlways = true;
            Console.WriteLine("Updated BuildPathWithSplitPartAlways: " + provider.BuildPathWithSplitPartAlways);
            workbook.Save("Output2", provider.SaveOptionsTemplate.SaveFormat);
        }
    }
}
```

### Ver también

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


