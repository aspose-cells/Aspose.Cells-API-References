---
title: "WorkbookSettings.WarningCallback"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Uyarı geri çağrısını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/workbooksettings/warningcallback/
---
## WorkbookSettings.WarningCallback property

Uyarı geri çağrısını alır veya ayarlar.

```csharp
public IWarningCallback WarningCallback { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyWarningCallbackDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Uyarı geri çağırmasını ayarla.
            workbook.Settings.WarningCallback = new WarningCallbackImplementation();

            // Potansiyel bir uyarı senaryosu (yinelenen adlandırılmış aralık) ile bir çalışma sayfası oluşturun
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Test");
            
            // Bu, yinelenen ad hakkında bir uyarı tetikleyecektir
            int index1 = workbook.Worksheets.Names.Add("TestRange");
            workbook.Worksheets.Names[index1].RefersTo = "=Sheet1!$A$1";
            
            int index2 = workbook.Worksheets.Names.Add("TestRange");
            workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$A$1";

            // Çalışma kitabını kaydedin (uyarı geri çağrısını tetikleyecek)
            workbook.Save("WarningCallbackExample.xlsx");
        }
    }

    public class WarningCallbackImplementation : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            Console.WriteLine($"Warning: {warningInfo.WarningType}, Description: {warningInfo.Description}");
        }
    }
}
```

### Ayrıca Bakınız

* interface [IWarningCallback](../../iwarningcallback/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


