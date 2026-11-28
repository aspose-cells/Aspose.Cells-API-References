---
title: "Workbook.HasCustomFunction"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook özelliği. Bu çalışma kitabında tanımlı adlardaki hücre formüllerinde kullanılan özel işlevin olup olmadığını algılar."
type: docs
url: /tr/net/aspose.cells/workbook/hascustomfunction/
---
## Workbook.HasCustomFunction property

Bu çalışma kitabında, hücre formüllerinde veya tanımlı adlarda kullanılan özel işlevlerin olup olmadığını algılar...

```csharp
public bool HasCustomFunction { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyHasCustomFunctionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            
            // Bir ada standart bir formül ekleyin.
            NameCollection names = wb.Worksheets.Names;
            int index = names.Add("StandardName");
            names[index].RefersTo = "=SUM(Sheet1!$A$1:$A$2)";
            Console.WriteLine($"Workbook has custom function (should be false): {wb.HasCustomFunction}");

            // Bir ada özel bir işlev ekleyin.
            index = names.Add("CustomName");
            names[index].RefersTo = "=MYFUNC()";
            Console.WriteLine($"Workbook has custom function (should be true): {wb.HasCustomFunction}");

            // Hücre formülleriyle test edin.
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Hücrede standart işlev.
            cells["A1"].Formula = "=SUM(B1:B2)";
            Console.WriteLine($"Cell has custom function (should be false): {cells["A1"].HasCustomFunction}");

            // Hücrede özel işlev.
            cells["A2"].Formula = "=MYFUNC(B1)";
            Console.WriteLine($"Cell has custom function (should be true): {cells["A2"].HasCustomFunction}");

            // Özel işlev içeren ada referans.
            cells["A3"].Formula = "=CustomName";
            Console.WriteLine($"Cell has custom function (should be true): {cells["A3"].HasCustomFunction}");

            // Birleştirilmiş özel işlevler.
            cells["A4"].Formula = "=MYFUNC(CustomName)";
            Console.WriteLine($"Cell has custom function (should be true): {cells["A4"].HasCustomFunction}");
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


