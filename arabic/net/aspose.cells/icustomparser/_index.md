---
title: "الواجهة ICustomParser"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الواجهة Aspose.Cells.ICustomParser. تسمح للمستخدمين بإضافة محلل القيم المخصص الخاص بهم لتحويل قيم السلسلة إلى كائن قيمة خلية مناسب آخر"
type: docs
url: /ar/net/aspose.cells/icustomparser/
---
## ICustomParser interface

يسمح للمستخدمين بإضافة محلل القيم المخصص الخاص بهم لتحويل قيم السلسلة إلى كائن قيمة خلية مناسب آخر.

```csharp
public interface ICustomParser
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| [GetFormat](../../aspose.cells/icustomparser/getformat/)() | يحصل على نمط التنسيق المقابل للقيمة التي تم تحليلها بواسطة آخر استدعاء لـ [`ParseObject`](./parseobject/). |
| [ParseObject](../../aspose.cells/icustomparser/parseobject/)(string) | يقوم بتحليل السلسلة المعطاة إلى كائن قيمة مناسب. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ICustomParserDemo
    {
        public static void ICustomParserExample()
        {
            // تنفيذ محلل مخصص
            ICustomParser customParser = new CustomParser();

            // مثال على استخدام طريقة ParseObject
            string valueToParse = "123.45";
            object parsedValue = customParser.ParseObject(valueToParse);
            Console.WriteLine($"Parsed Value: {parsedValue}");

            // مثال على استخدام طريقة GetFormat
            string format = customParser.GetFormat();
            Console.WriteLine($"Format: {format}");
        }
    }

    // تنفيذ مخصص للواجهة ICustomParser
    public class CustomParser : ICustomParser
    {
        private string lastFormat;

        public object ParseObject(string value)
        {
            // منطق تحليل مثال
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

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


