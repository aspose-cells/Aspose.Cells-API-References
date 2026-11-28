---
title: "CopyOptions.CopyNames"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CopyOptions özelliği. İsimlerin kopyalanıp kopyalanmayacağını gösterir"
type: docs
url: /tr/net/aspose.cells/copyoptions/copynames/
---
## CopyOptions.CopyNames property

İsimlerin kopyalanıp kopyalanmayacağını gösterir.

```csharp
public bool CopyNames { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyCopyNamesDemo
    {
        public static void Run()
        {
            // Adlandırılmış aralıklarla bir kaynak çalışma kitabı oluştur
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            
            // Kaynak çalışma kitabında adlandırılmış bir aralık oluştur
            sourceSheet.Cells["A1"].PutValue("Test Value");
            int index = sourceWorkbook.Worksheets.Names.Add("SourceName");
            sourceWorkbook.Worksheets.Names[index].RefersTo = "=Sheet1!$A$1";

            // Bir hedef çalışma kitabı oluştur
            Workbook destWorkbook = new Workbook();
            
            // CopyNames=true ile çalışma sayfasını kopyala
            destWorkbook.Worksheets[0].Copy(sourceSheet, new CopyOptions { CopyNames = true });

            // İsimlendirilmiş aralığın kopyalandığını doğrulayın
            Name copiedName = destWorkbook.Worksheets.Names["SourceName"];
            if (copiedName != null)
            {
                Console.WriteLine("Named range copied successfully: " + copiedName.RefersTo);
            }
            else
            {
                Console.WriteLine("Named range was not copied");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


