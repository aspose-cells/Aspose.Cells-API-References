---
title: "WriteProtection.Author"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WriteProtection özelliği. Yazarını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/writeprotection/author/
---
## WriteProtection.Author property

Yazarı alır ve ayarlar.

```csharp
public string Author { get; set; }
```

### Örnekler

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

            // Author özelliğinin kullanımını göster
            writeProtection.Author = "John Doe";
            writeProtection.Password = "password123";
            
            Console.WriteLine("Write protection author: " + writeProtection.Author);
            Console.WriteLine("Is write protected: " + writeProtection.IsWriteProtected);

            workbook.Save("WriteProtectionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


