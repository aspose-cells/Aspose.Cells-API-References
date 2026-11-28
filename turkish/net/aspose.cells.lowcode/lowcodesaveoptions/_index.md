---
title: "Sınıf LowCodeSaveOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.LowCode.LowCodeSaveOptions sınıfı. Oluşturulan sonuçları düşük kod yöntemiyle kaydetmek için seçenekler"
type: docs
url: /tr/net/aspose.cells.lowcode/lowcodesaveoptions/
---
## LowCodeSaveOptions class

Düşük kodlu bir şekilde oluşturulan sonuçları kaydetme seçenekleri.

```csharp
public class LowCodeSaveOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [LowCodeSaveOptions](lowcodesaveoptions/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [OutputFile](../../aspose.cells.lowcode/lowcodesaveoptions/outputfile/) { get; set; } | Oluşturulan verileri kaydetmek için dosyayı (gerekirse yol ile) alır ve ayarlar. Bu özelliği null veya boş dize dışındaki bir değerle ayarladığınızda, [`OutputStream`](./outputstream/) yok sayılacaktır. |
| [OutputStream](../../aspose.cells.lowcode/lowcodesaveoptions/outputstream/) { get; set; } | Oluşturulan verileri yazmak için akışı alır ve ayarlar. Bu özelliği null dışındaki bir değerle ayarladığınızda, [`OutputFile`](./outputfile/) yok sayılacaktır. |
| virtual [SaveFormat](../../aspose.cells.lowcode/lowcodesaveoptions/saveformat/) { get; set; } | Çıktı için kaydetme formatını alır ve ayarlar. Genel olarak, düşük kod yöntemiyle belirli bir işlem için yalnızca bazı belirli formatlara izin verilir. Lütfen ilgili işlem için doğru formatı belirtin, aksi takdirde beklenmeyen sonuçlar veya hatta istisna oluşabilir. |

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodeClassLowCodeSaveOptionsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bir çalışma sayfası ekleyin ve bazı veriler yerleştirin
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // Kaydetme seçeneklerini oluşturun
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions()
            {
                OutputFile = "output.xlsx"
            };

            // Çalışma kitabını belirtilen seçenekleri kullanarak kaydedin
            workbook.Save(saveOptions.OutputFile, saveOptions.SaveFormat);
            
            Console.WriteLine("File saved successfully with LowCodeSaveOptions");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


