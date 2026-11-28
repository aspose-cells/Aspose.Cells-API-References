---
title: "LowCodeSaveOptions.OutputStream"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LowCodeSaveOptions özelliği. Oluşturulan verileri yazmak için akışı alır ve ayarlar. Bu özelliği null olmayan bir değerle ayarladığınızda OutputFile yok sayılacaktır"
type: docs
url: /tr/net/aspose.cells.lowcode/lowcodesaveoptions/outputstream/
---
## LowCodeSaveOptions.OutputStream property

Oluşturulan verileri yazmak için akışı alır ve ayarlar. Bu özelliği null olmayan bir değerle ayarladığınızda, [`OutputFile`](../outputfile/) yok sayılacaktır.

```csharp
public Stream OutputStream { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class LowCodeSaveOptionsPropertyOutputStreamDemo
    {
        public static void Run()
        {
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample OutputStream Demo");

            try
            {
                // LowCodeSaveOptions örneği oluşturun
                LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
                
                // Demonstrasyon için bir bellek akışı oluşturun
                using (MemoryStream stream = new MemoryStream())
                {
                    // OutputStream özelliğini ayarlayın
                    saveOptions.OutputStream = stream;
                    saveOptions.SaveFormat = SaveFormat.Xlsx;

                    // Seçenekleri kullanarak kaydedin (bellek akışımıza yazılacak)
                    workbook.Save(saveOptions.OutputStream, saveOptions.SaveFormat);

                    // Akışın yazıldığını doğrulayın
                    Console.WriteLine($"OutputStream length: {saveOptions.OutputStream.Length} bytes");
                    Console.WriteLine("OutputStream position reset to 0 for reading");
                    saveOptions.OutputStream.Position = 0;

                    // İçeriği doğrulamak için akıştan yeni bir çalışma kitabı oluşturun
                    Workbook verifyWorkbook = new Workbook(saveOptions.OutputStream);
                    Console.WriteLine($"Verified worksheet count: {verifyWorkbook.Worksheets.Count}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [LowCodeSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


