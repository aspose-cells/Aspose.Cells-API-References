---
title: "ICustomParser.GetFormat"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ICustomParser. يحصل على نمط التنسيق المقابل للقيمة التي تم تحليلها بواسطة آخر استدعاء لـ ParseObject"
type: docs
url: /ar/net/aspose.cells/icustomparser/getformat/
---
## ICustomParser.GetFormat method

يحصل على نمط التنسيق المقابل للقيمة التي تم تحليلها بواسطة آخر استدعاء لـ [`ParseObject`](../parseobject/).

```csharp
public string GetFormat()
```

### ملاحظات

قد يُستخدم نمط التنسيق المُرجع لتنسيق الخلية المقابلة (اضبطها إلى Style.Custom للخلية).

### أمثلة

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

### انظر أيضًا

* interface [ICustomParser](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


