---
title: "MetadataOptions.MetadataOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MetadataOptions yapıcı. Meta veriyi yüklemek için bir seçenek oluşturur"
type: docs
url: /tr/net/aspose.cells.metadata/metadataoptions/metadataoptions/
---
## MetadataOptions constructor

Meta veriyi yükleme seçeneklerini oluşturur.

```csharp
public MetadataOptions(MetadataType metadataType)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| metadataType | MetadataType | Meta veri türü. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metadata;
    using System;

    public class MetadataOptionsMethodCtorWithMetadataTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // #ctor metodunu MetadataType parametresiyle çağır
                MetadataOptions options = new MetadataOptions(MetadataType.Encryption);
                
                // Ek özellikleri ayarla
                options.Password = "test123";
                options.KeyLength = 128;
                
                // Oluşturulan seçenekleri göster
                Console.WriteLine($"MetadataType: {options.MetadataType}");
                Console.WriteLine($"Password set: {!string.IsNullOrEmpty(options.Password)}");
                Console.WriteLine($"KeyLength: {options.KeyLength}");

                // Meta veri yüklerken seçenekleri kullan (örnek)
                // Bu genellikle bir dosya açarken LoadOptions ile kullanılır
                // Not: Orijinal kod MetadataOptions'ı doğrudan LoadOptions üzerine ayarlamaya çalıştı,
                // ancak LoadOptions sınıfının sağlanan tanımda bu özelliği yoktur.
                // LoadOptions ile kullanım olduğu için sadece seçenek oluşturma kısmını tutacağız
                // Mevcut API tanımıyla mümkün değil.
                
                Console.WriteLine("MetadataOptions created successfully with MetadataType parameter");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating MetadataOptions: {ex.Message}");
            }
            
            // Çalışma kitabını kaydet (ancak meta veri seçenekleri bu boş çalışma kitabını etkilemez)
            workbook.Save("MetadataOptionsCtorDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [MetadataType](../../metadatatype/)
* class [MetadataOptions](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


