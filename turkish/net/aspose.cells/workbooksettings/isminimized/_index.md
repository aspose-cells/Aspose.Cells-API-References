---
title: "WorkbookSettings.IsMinimized"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Oluşturulan elektronik tablonun Küçültülmüş olarak açılıp açılmayacağını temsil eder"
type: docs
url: /tr/net/aspose.cells/workbooksettings/isminimized/
---
## WorkbookSettings.IsMinimized property

Oluşturulan elektronik tablonun Küçültülmüş olarak açılıp açılmayacağını temsil eder.

```csharp
public bool IsMinimized { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsMinimizedDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // IsMinimized özelliğini true olarak ayarla
            workbook.Settings.IsMinimized = true;

            // Çalışma kitabını kaydedin
            workbook.Save("IsMinimizedDemo.xlsx");

            // Kaydedilmiş çalışma kitabını yükleyerek özelliği doğrulayın
            Workbook loadedWorkbook = new Workbook("IsMinimizedDemo.xlsx");

            // IsMinimized özelliğinin değerini çıktı olarak ver
            Console.WriteLine("Workbook IsMinimized property: " + loadedWorkbook.Settings.IsMinimized);
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


