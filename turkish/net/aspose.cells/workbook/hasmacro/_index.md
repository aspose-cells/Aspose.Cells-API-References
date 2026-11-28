---
title: "Workbook.HasMacro"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook özelliği. Bu elektronik tablonun makro/VBA içerip içermediğini gösterir"
type: docs
url: /tr/net/aspose.cells/workbook/hasmacro/
---
## Workbook.HasMacro property

Bu elektronik tablonun makro/VBA içerip içermediğini gösterir.

```csharp
public bool HasMacro { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyHasMacroDemo
    {
        public static void Run()
        {
            // Şablon dosyası yükleyerek makro içeren bir çalışma kitabı oluştur
            Workbook workbookWithMacro = new Workbook("sample_with_macro.xlsm");
            Console.WriteLine("Workbook with macro - HasMacro: " + workbookWithMacro.HasMacro);

            // Makro olmadan bir çalışma kitabı oluştur
            Workbook workbookWithoutMacro = new Workbook();
            Console.WriteLine("Workbook without macro - HasMacro: " + workbookWithoutMacro.HasMacro);
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


