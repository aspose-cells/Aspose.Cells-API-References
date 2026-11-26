---
title: "NumbersLoadOptions.NumbersLoadOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor NumbersLoadOptions. Constructor"
type: docs
url: /es/net/aspose.cells.numbers/numbersloadoptions/numbersloadoptions/
---
## NumbersLoadOptions constructor

Constructor.

```csharp
public NumbersLoadOptions()
```

### Ejemplos

```csharp
using System;
using System.Globalization;
using Aspose.Cells;
using Aspose.Cells.Numbers;

namespace AsposeCellsExamples
{
    public class NumbersLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crear NumbersLoadOptions usando el constructor
            NumbersLoadOptions loadOptions = new NumbersLoadOptions
            {
                // Establecer algunas propiedades comunes
                Password = "secure123",
                ParsingFormulaOnOpen = true,
                CultureInfo = new CultureInfo("en-US"),
                StandardFont = "Arial",
                MemorySetting = MemorySetting.MemoryPreference
            };

            // Cargue el libro de trabajo con las opciones
            Workbook workbook = new Workbook("sample.numbers", loadOptions);

            // Guardar como XLSX
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [NumbersLoadOptions](../)
* namespace [Aspose.Cells.Numbers](../../../aspose.cells.numbers/)
* assembly [Aspose.Cells](../../../)


