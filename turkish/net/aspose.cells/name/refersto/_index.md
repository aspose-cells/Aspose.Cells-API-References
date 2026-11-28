---
title: "Name.RefersTo"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Name özelliği. İsim tanımlandığında eşittir işaretiyle başlayan formülü döndürür veya ayarlar"
type: docs
url: /tr/net/aspose.cells/name/refersto/
---
## Name.RefersTo property

Adın referans vermek üzere tanımlandığı formülü, eşittir işaretiyle başlayan, alır veya ayarlar.

```csharp
public string RefersTo { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyRefersToDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "Sheet1";

            // RefersTo ile adlandırılmış aralıklar ekle
            int index1 = workbook.Worksheets.Names.Add("NamedRange1");
            workbook.Worksheets.Names[index1].RefersTo = "=Sheet1!$6:$8";
            
            int index2 = workbook.Worksheets.Names.Add("NamedRange2");
            workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$C:$D";

            // Adlandırılmış aralıkların RefersTo özelliğini göster
            Console.WriteLine("NamedRange1 RefersTo: " + workbook.Worksheets.Names[0].RefersTo);
            Console.WriteLine("NamedRange2 RefersTo: " + workbook.Worksheets.Names[1].RefersTo);
        }
    }
}
```

### Ayrıca Bakınız

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


