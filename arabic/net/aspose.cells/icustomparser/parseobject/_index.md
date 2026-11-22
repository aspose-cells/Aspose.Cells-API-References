---
title: "ICustomParser.ParseObject"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ICustomParser. يحلل السلسلة المعطاة إلى كائن قيمة مناسب"
type: docs
url: /ar/net/aspose.cells/icustomparser/parseobject/
---
## ICustomParser.ParseObject method

يقوم بتحليل السلسلة المعطاة إلى كائن قيمة مناسب.

```csharp
public object ParseObject(string value)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | String | القيمة النصية التي سيتم تحليلها |

### قيمة الإرجاع

كائن قيمة تم تحليله من السلسلة المعطاة. إذا تعذّر تحليل السلسلة المعطاة إلى كائن قيمة مناسب، يُرجع null.

### أمثلة

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

### انظر أيضًا

* interface [ICustomParser](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


