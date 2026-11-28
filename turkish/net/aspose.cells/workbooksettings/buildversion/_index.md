---
title: "WorkbookSettings.BuildVersion"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Uygulamanın artımlı genel sürümünü belirtir"
type: docs
url: /tr/net/aspose.cells/workbooksettings/buildversion/
---
## WorkbookSettings.BuildVersion property

Uygulamanın artımlı genel sürümünü belirtir.

```csharp
public string BuildVersion { get; set; }
```

### Örnekler

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyBuildVersionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // WorkbookSettings'a erişin.
            WorkbookSettings settings = workbook.Settings;
            
            // Temel ayarları ayarlayın
            settings.Author = "Sample Author";
            settings.CultureInfo = new CultureInfo("en-US");
            
            // BuildVersion özelliğini gösterin
            settings.BuildVersion = "2.5.0";
            Console.WriteLine($"Build Version set to: {settings.BuildVersion}");
            
            // Çalışma kitabını kaydedin
            workbook.Save("BuildVersionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


