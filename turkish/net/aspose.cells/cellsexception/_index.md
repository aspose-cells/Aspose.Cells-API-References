---
title: "Sınıf CellsException"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.CellsException sınıfı. Aspose.Cells tarafından belirtilen bir hata oluştuğunda atılan istisna"
type: docs
url: /tr/net/aspose.cells/cellsexception/
---
## CellsException class

Aspose.Cells belirtilen bir hata oluştuğunda fırlatılan istisna.

```csharp
public class CellsException : ApplicationException
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Code](../../aspose.cells/cellsexception/code/) { get; } | Özel istisna kodunu temsil eder. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;
    using System.Collections;

    public class CellsExceptionDemo
    {
        public static void CellsExceptionExample()
        {
            try
            {
                // Bir istisna oluşturan bir işlemi simüle edin
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                // Geçersiz bir hücreye erişerek kasıtlı olarak bir istisna oluşturma
                Cell cell = worksheet.Cells["InvalidCellAddress"];
            }
            catch (CellsException ex)
            {
                // CellsException'ı ele al
                Console.WriteLine("Aspose.Cells.CellsException caught!");
                Console.WriteLine($"Code: {ex.Code}");
                Console.WriteLine($"Message: {ex.Message}");
                Console.WriteLine($"TargetSite: {ex.TargetSite}");
                Console.WriteLine($"StackTrace: {ex.StackTrace}");
                Console.WriteLine($"HelpLink: {ex.HelpLink}");
                Console.WriteLine($"Source: {ex.Source}");
                Console.WriteLine($"HResult: {ex.HResult}");
                if (ex.InnerException != null)
                {
                    Console.WriteLine($"InnerException: {ex.InnerException.Message}");
                }
                foreach (DictionaryEntry entry in ex.Data)
                {
                    Console.WriteLine($"Data: {entry.Key} = {entry.Value}");
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


