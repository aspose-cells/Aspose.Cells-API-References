---
title: "AbstractLowCodeLoadOptionsProvider.Current"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AbstractLowCodeLoadOptionsProvider özelliği. Şu anda işlenen kısmın verilerini yüklemek için kullanılan yükleme seçeneklerini alır"
type: docs
url: /tr/net/aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/current/
---
## AbstractLowCodeLoadOptionsProvider.Current property

Şu anda işlenen parçanın verilerini yüklemek için kullanılacak yükleme seçeneklerini alır.

```csharp
public abstract LowCodeLoadOptions Current { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.Collections;

    public class AbstractLowCodeLoadOptionsProviderPropertyCurrentDemo
    {
        public static void Run()
        {
            string[] files = { "file1.xlsx", "file2.xlsx", "file3.xlsx" };
            // Özel sağlayıcıyı yükleme seçeneklerimizle başlat
            CustomProvider provider = new CustomProvider(files);
            
            int counter = 1;
            while (provider.MoveNext())
            {
                // Aktif yükleme seçeneklerini almak için Current özelliğine eriş
                Console.WriteLine($"Processing set {counter}");
                    
                // Mevcut yükleme seçeneklerinin girdi dosyası/akışını kullanarak çalışma kitabı oluştur
                Workbook workbook;
                if (provider.Current.InputFile != null)
                {
                    workbook = new Workbook(provider.Current.InputFile);
                }
                else if (provider.Current.InputStream != null)
                {
                    workbook = new Workbook(provider.Current.InputStream);
                }
                else
                {
                    workbook = new Workbook();
                }

                Worksheet worksheet = workbook.Worksheets[0];

                // Eksik özellik nedeniyle kaldırılan seçenek etkisini göster
                worksheet.Cells["A1"].Value = "Sample Value";

                // Sonucu kaydedin
                workbook.Save($"CurrentDemo_{counter}.xlsx");
                counter++;
            }
        }
    }

    // IDisposable ile özel sağlayıcı uygulaması
    public class CustomProvider : AbstractLowCodeLoadOptionsProvider
    {
        
        public IEnumerator fileIter;

        public CustomProvider(string[] files)
        {
            fileIter = files.GetEnumerator();
            current = new LowCodeLoadOptions();
        }
        private LowCodeLoadOptions current;

        public override LowCodeLoadOptions Current => current;

        public override bool MoveNext()
        {
            if (fileIter.MoveNext())
            {
                current = new LowCodeLoadOptions();
                current.InputFile = fileIter.Current.ToString();
                return true;
            }

            return false;
        }

        public override void Finish(LowCodeLoadOptions part)
        {
            base.Finish(part);
        }

    }
}
```

### Ayrıca Bakınız

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [AbstractLowCodeLoadOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


