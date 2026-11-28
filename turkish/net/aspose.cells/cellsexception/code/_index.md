---
title: "CellsException.Code"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellsException özelliği. Özel istisna kodunu temsil eder"
type: docs
url: /tr/net/aspose.cells/cellsexception/code/
---
## CellsException.Code property

Özel istisna kodunu temsil eder.

```csharp
public ExceptionType Code { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsExceptionPropertyCodeDemo
    {
        public static void Run()
        {
            try
            {
                // Bir çalışma kitabı oluştur ve var olmayan bir çalışma sayfasına erişmeye çalış
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets["NonExistentSheet"];
            }
            catch (CellsException e)
            {
                // Code özelliğinin kullanımını gösterin
                Console.WriteLine($"Error Code: {e.Code}");
                Console.WriteLine($"Error Message: {e.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [ExceptionType](../../exceptiontype/)
* class [CellsException](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


