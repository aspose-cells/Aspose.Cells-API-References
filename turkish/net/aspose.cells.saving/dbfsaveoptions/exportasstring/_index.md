---
title: "DbfSaveOptions.ExportAsString"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DbfSaveOptions özelliği. Değerin string olarak dışa aktarılıp aktarılmayacağını gösterir"
type: docs
url: /tr/net/aspose.cells.saving/dbfsaveoptions/exportasstring/
---
## DbfSaveOptions.ExportAsString property

Dizgi değeri olarak dışa aktarmayı belirtir

```csharp
public bool ExportAsString { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class DbfSaveOptionsPropertyExportAsStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Karışık tiplerde örnek veri ekle
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(123.45);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("TextValue");

            // DbfSaveOptions örneği oluştur
            DbfSaveOptions options = new DbfSaveOptions();

            // Mevcut ExportAsString değerini göster
            Console.WriteLine("Current ExportAsString value: " + options.ExportAsString);

            // ExportAsString'i true olarak ayarla (tüm değerler string olarak dışa aktarılacak)
            options.ExportAsString = true;
            Console.WriteLine("ExportAsString set to: " + options.ExportAsString);

            // ExportAsString = true ile kaydet
            workbook.Save("ExportAsStringTrue.dbf", options);

            // ExportAsString'i false olarak ayarla (değerler özgün tiplerini koruyacak)
            options.ExportAsString = false;
            Console.WriteLine("ExportAsString set to: " + options.ExportAsString);

            // ExportAsString = false ile kaydet
            workbook.Save("ExportAsStringFalse.dbf", options);
        }
    }
}
```

### Ayrıca Bakınız

* class [DbfSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


