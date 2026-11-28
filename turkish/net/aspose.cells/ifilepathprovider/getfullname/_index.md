---
title: "IFilePathProvider.GetFullName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "IFilePathProvider yöntemi. Çalışma Sayfası adını kullanarak dosyanın tam yolunu alır ve Çalışma Sayfasını ayrı ayrı HTML'ye dışa aktarırken referansların doğru şekilde dışa aktarılmasını sağlar"
type: docs
url: /tr/net/aspose.cells/ifilepathprovider/getfullname/
---
## IFilePathProvider.GetFullName method

Çalışma Sayfasını ayrı ayrı HTML olarak dışa aktarırken, dosyanın tam yolunu Çalışma Sayfası adıyla alır. Böylece Çalışma Sayfaları arasındaki referanslar doğru şekilde dışa aktarılabilir.

```csharp
public string GetFullName(string sheetName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetName | String | Çalışma sayfası adı |

### Dönüş Değeri

dosyanın tam yolu

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IFilePathProviderMethodGetFullNameWithStringDemo
    {
        public static void Run()
        {
            // IFilePathProvider için özel bir uygulama oluştur
            CustomFilePathProvider provider = new CustomFilePathProvider();

            // GetFullName yöntemini bir sayfa adıyla çağır
            string sheetName = "Sheet1";
            string fullPath = provider.GetFullName(sheetName);

            // Sonucu göster
            Console.WriteLine($"Full path for {sheetName}: {fullPath}");
        }
    }

    internal class CustomFilePathProvider : IFilePathProvider
    {
        public string GetFullName(string sheetName)
        {
            // Sayfa adını bir dizinle birleştirerek bir yol döndüren basit uygulama
            return $"C:\\Temp\\{sheetName}.xlsx";
        }
    }
}
```

### Ayrıca Bakınız

* interface [IFilePathProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


