---
title: "WorkbookSettings.StreamProvider"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Harici kaynak için akış sağlayıcısını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/workbooksettings/streamprovider/
---
## WorkbookSettings.StreamProvider property

Harici kaynak için akış sağlayıcısını alır ve ayarlar.

```csharp
[Obsolete("Use ResourceProvider property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IStreamProvider StreamProvider { get; set; }
```

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen ResourceProvider özelliğini kullanın. Bu özellik, Haziran 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CustomStreamProvider1 : IStreamProvider
    {
        private MemoryStream stream;

        public void InitStream(StreamProviderOptions options)
        {
            stream = new MemoryStream();
            options.Stream = stream;
        }

        public void CloseStream(StreamProviderOptions options)
        {
            stream.Close();
            Console.WriteLine($"Stream closed. Content length: {stream.Length} bytes");
        }
    }

    public class WorkbookSettingsPropertyStreamProviderDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma kitabı ayarlarına eriş
            WorkbookSettings settings = workbook.Settings;

            // Mevcut StreamProvider değerini göster
            Console.WriteLine("Current StreamProvider value: " + (settings.StreamProvider == null ? "null" : "custom provider"));

            // Özel bir akış sağlayıcı ayarla
            settings.StreamProvider = new CustomStreamProvider1();

            // Akış kullanımını göstermek için bazı veriler ekle
            worksheet.Cells["A1"].PutValue("Test data for stream provider");

            // Çalışma kitabını kaydet - bu, akış sağlayıcıyı tetikleyecek
            workbook.Save("PropertyStreamProviderDemo.xlsx");

            // Akış sağlayıcıyı sıfırla
            settings.StreamProvider = null;
            Console.WriteLine("StreamProvider reset to null");
        }
    }
}
```

### Ayrıca Bakınız

* interface [IStreamProvider](../../istreamprovider/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


