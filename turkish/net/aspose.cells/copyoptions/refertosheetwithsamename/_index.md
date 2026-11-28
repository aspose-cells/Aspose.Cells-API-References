---
title: "CopyOptions.ReferToSheetWithSameName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CopyOptions özelliği. MS Excel'de, başka çalışma sayfalarına başvuran formüller bir çalışma sayfası başka birine kopyalanırken, kopyalanan formüllerin kaynak çalışma kitabına başvurması gerekir. Ancak bazı durumlarda kullanıcı, kopyalanan formüllerin aynı çalışma kitabında aynı ada sahip çalışma sayfalarına başvurmasını isteyebilir; örneğin bu çalışma sayfaları daha önce bu kopyalama işlemi sırasında kopyalanmışsa, bu özellik true olarak tutulmalıdır."
type: docs
url: /tr/net/aspose.cells/copyoptions/refertosheetwithsamename/
---
## CopyOptions.ReferToSheetWithSameName property

MS Excel'de, bir çalışma sayfasını başka birine kopyalarken diğer çalışma sayfalarına referans veren formüller kopyalandığında, kopyalanan formüllerin kaynak çalışma kitabına referans vermesi gerekir. Ancak bazı durumlarda kullanıcı, kopyalanan formüllerin aynı çalışma kitabındaki aynı ada sahip çalışma sayfalarına referans vermesini isteyebilir; örneğin bu çalışma sayfaları bu kopyalama işleminden önce zaten kopyalanmışsa, bu özellik true olarak tutulmalıdır.

```csharp
public bool ReferToSheetWithSameName { get; set; }
```

### Açıklamalar

Varsayılan değer true'tur.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyReferToSheetWithSameNameDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir şablon çalışma kitabı oluşturun
            Workbook templateWorkbook = new Workbook();
            Worksheet templateSheet1 = templateWorkbook.Worksheets[0];
            templateSheet1.Name = "Data";
            templateSheet1.Cells["A1"].PutValue("Value");
            templateSheet1.Cells["A2"].PutValue(10);
            templateSheet1.Cells["A3"].PutValue(20);
            
            Worksheet templateSheet2 = templateWorkbook.Worksheets.Add("Summary");
            templateSheet2.Cells["B2"].Formula = "=SUM(Data!A2:A3)";

            // Çıktı çalışma kitabını oluşturun
            Workbook outputWorkbook = new Workbook();
            outputWorkbook.Worksheets.Clear();

            // ReferToSheetWithSameName etkinleştirilmiş şekilde çalışma sayfalarını kopyalayın
            foreach (Worksheet sheet in templateWorkbook.Worksheets)
            {
                outputWorkbook.Worksheets.Add(sheet.Name);
                CopyOptions options = new CopyOptions();
                options.ReferToSheetWithSameName = true;
                outputWorkbook.Worksheets[sheet.Name].Copy(sheet, options);
            }

            // Formülün doğru sayfaya başvurduğunu doğrulayın
            Console.WriteLine("Formula in output workbook: " + 
                outputWorkbook.Worksheets["Summary"].Cells["B2"].Formula);
        }
    }
}
```

### Ayrıca Bakınız

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


