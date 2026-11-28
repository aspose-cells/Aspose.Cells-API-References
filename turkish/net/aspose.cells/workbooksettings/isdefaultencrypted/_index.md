---
title: "WorkbookSettings.IsDefaultEncrypted"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Çalışma kitabının Yapısı ve Pencereleri kilitli olduğunda varsayılan şifreyle şifrelenip şifrelenmediğini gösterir"
type: docs
url: /tr/net/aspose.cells/workbooksettings/isdefaultencrypted/
---
## WorkbookSettings.IsDefaultEncrypted property

Çalışma kitabının Yapısı ve Pencereleri kilitli ise varsayılan şifreyle şifrelenip şifrelenmediğini gösterir.

```csharp
public bool IsDefaultEncrypted { get; set; }
```

### Açıklamalar

Varsayılan değer artık false. MS Excel 2013 ile aynı.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsDefaultEncryptedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook(FileFormatType.Xlsx);
            Console.WriteLine("IsDefaultEncrypted: " + workbook.Settings.IsDefaultEncrypted);
            
            workbook.Settings.IsDefaultEncrypted = true;
            Console.WriteLine("After setting to true: " + workbook.Settings.IsDefaultEncrypted);
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


