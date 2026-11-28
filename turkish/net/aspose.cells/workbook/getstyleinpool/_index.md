---
title: "Workbook.GetStyleInPool"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Stil havuzundaki stili alır. Çalışma kitabındaki tüm stiller bir havuza toplanır. Hücrelerde yalnızca basit bir referans indeksi bulunur."
type: docs
url: /tr/net/aspose.cells/workbook/getstyleinpool/
---
## Workbook.GetStyleInPool method

Stil havuzundaki stili alır. Çalışma kitabındaki tüm stiller bir havuza toplanacaktır. Hücrelerde yalnızca basit bir referans indeksi bulunur.

```csharp
public Style GetStyleInPool(int index)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| indeks | Int32 | İndeks. |

### Dönüş Değeri

Havuzdaki stil verilen indekse karşılık gelir, null olabilir.

### Açıklamalar

Eğer döndürülen stil değiştirilirse, bu stile referans veren tüm hücrelerin stili değişir.

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodGetStyleInPoolWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            
            // İlk çalışma sayfasına eriş ve bazı örnek veriler ekle
            Worksheet ws = wb.Worksheets[0];
            ws.Cells["A1"].PutValue("Sample Data");
            ws.Cells["A2"].PutValue(123.45);
            ws.Cells["A3"].PutValue(DateTime.Now);
            
            // Bazı stilleri uygula
            Style style1 = wb.CreateStyle();
            style1.Custom = "$#,##0.00";
            ws.Cells["A2"].SetStyle(style1);
            
            Style style2 = wb.CreateStyle();
            style2.Custom = "yyyy-mm-dd";
            ws.Cells["A3"].SetStyle(style2);
            
            // Bellek akışına kaydet
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Xlsx);
                
                // Çalışma kitabını akıştan yeniden yükle
                ms.Position = 0;
                Workbook reloadWb = new Workbook(ms);
                
                // Stil havuzundan stilleri al ve göster
                int count = reloadWb.CountOfStylesInPool;
                Console.WriteLine($"Styles in pool: {count}");
                
                for (int i = 0; i < count; i++)
                {
                    Style style = reloadWb.GetStyleInPool(i);
                    Console.WriteLine($"Style {i}: CustomFormat={style.Custom}");
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


