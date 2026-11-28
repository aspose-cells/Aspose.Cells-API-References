---
title: "ICustomParser.ParseObject"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ICustomParser yöntemi. Verilen dizeyi uygun değer nesnesine ayrıştırır"
type: docs
url: /tr/net/aspose.cells/icustomparser/parseobject/
---
## ICustomParser.ParseObject method

Verilen dizeyi uygun değer nesnesine ayrıştırır.

```csharp
public object ParseObject(string value)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | String | Ayrıştırılacak dize değeri |

### Dönüş Değeri

Verilen dizeden ayrıştırılan değer nesnesi. Verilen dize uygun değer nesnesine ayrıştırılamazsa, null döndürür.

### Örnekler

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{

    public class CustomParser : ICustomParser
    {
        public object ParseObject(string s)
        {
            if (double.TryParse(s, out double result))
            {
                return result;
            }
            return s;
        }

        public string GetFormat()
        {
            return "Numeric or string format";
        }
    }

    public class ICustomParserMethodParseObjectWithStringDemo
    {
        public static void Run()
        {
            ICustomParser customParser = new CustomParser();
            string valueToParse = "123.45";
            object parsedValue = customParser.ParseObject(valueToParse);
            Console.WriteLine($"Parsed Value: {parsedValue}");

            string format = customParser.GetFormat();
            Console.WriteLine($"Format: {format}");
        }
    }
}
```

### Ayrıca Bakınız

* interface [ICustomParser](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


