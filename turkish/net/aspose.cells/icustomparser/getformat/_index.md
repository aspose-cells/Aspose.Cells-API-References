---
title: "ICustomParser.GetFormat"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ICustomParser yöntemi. ParseObject'in son çağrısı tarafından ayrıştırılan değere karşılık gelen biçimlendirme desenini alır"
type: docs
url: /tr/net/aspose.cells/icustomparser/getformat/
---
## ICustomParser.GetFormat method

[`ParseObject`](../parseobject/) çağrısının son gerçekleşmesiyle ayrıştırılan değere karşılık gelen biçimlendirme desenini alır.

```csharp
public string GetFormat()
```

### Açıklamalar

Dönen biçimlendirme deseni, ilgili hücreyi biçimlendirmek için kullanılabilir (hücre için Style.Custom olarak ayarlayın).

### Örnekler

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
   
    public class CustomParser2 : ICustomParser
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
            return "Standard numeric format";
        }
    }

    public class ICustomParser1MethodGetFormatDemo
    {
        public static void Run()
        {
            ICustomParser customParser = new CustomParser2();

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


