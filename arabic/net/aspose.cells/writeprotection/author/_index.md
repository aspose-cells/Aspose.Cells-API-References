---
title: "WriteProtection.Author"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WriteProtection. يحصل وتعيّن المؤلف"
type: docs
url: /ar/net/aspose.cells/writeprotection/author/
---
## WriteProtection.Author property

يحصل على المؤلف ويضبطه.

```csharp
public string Author { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WriteProtectionPropertyAuthorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WorkbookSettings settings = workbook.Settings;
            WriteProtection writeProtection = settings.WriteProtection;

            // إظهار استخدام خاصية Author
            writeProtection.Author = "John Doe";
            writeProtection.Password = "password123";
            
            Console.WriteLine("Write protection author: " + writeProtection.Author);
            Console.WriteLine("Is write protected: " + writeProtection.IsWriteProtected);

            workbook.Save("WriteProtectionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


