---
title: "Arayüz ICustomParser"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ICustomParser arayüzü. Kullanıcıların dize değerlerini diğer uygun hücre değeri nesnesine ayrıştırmak için özel değer ayrıştırıcılarını eklemelerine olanak tanır"
type: docs
url: /tr/net/aspose.cells/icustomparser/
---
## ICustomParser interface

Kullanıcıların dize değerlerini diğer uygun hücre değeri nesnelerine ayrıştırmak için özel değer ayrıştırıcılarını eklemelerine izin verir.

```csharp
public interface ICustomParser
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [GetFormat](../../aspose.cells/icustomparser/getformat/)() | Son [`ParseObject`](./parseobject/) çağrısı ile ayrıştırılan değere karşılık gelen biçimlendirme desenini alır. |
| [ParseObject](../../aspose.cells/icustomparser/parseobject/)(string) | Verilen dizeyi uygun değer nesnesine ayrıştırır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ICustomParserDemo
    {
        public static void ICustomParserExample()
        {
            // Özel ayrıştırıcı uygulaması
            ICustomParser customParser = new CustomParser();

            // ParseObject yöntemi örnek kullanımı
            string valueToParse = "123.45";
            object parsedValue = customParser.ParseObject(valueToParse);
            Console.WriteLine($"Parsed Value: {parsedValue}");

            // GetFormat yöntemi örnek kullanımı
            string format = customParser.GetFormat();
            Console.WriteLine($"Format: {format}");
        }
    }

    // ICustomParser için özel uygulama
    public class CustomParser : ICustomParser
    {
        private string lastFormat;

        public object ParseObject(string value)
        {
            // Örnek ayrıştırma mantığı
            if (double.TryParse(value, out double result))
            {
                lastFormat = "0.00"; // Example format
                return result;
            }
            lastFormat = null;
            return null;
        }

        public string GetFormat()
        {
            return lastFormat;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


