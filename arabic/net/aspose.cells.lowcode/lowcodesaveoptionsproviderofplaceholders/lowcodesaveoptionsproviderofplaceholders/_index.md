---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.LowCodeSaveOptionsProviderOfPlaceHolders"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ LowCodeSaveOptionsProviderOfPlaceHolders. ينشئ نسخة لتوفير خيارات الحفظ وفقًا للقوالب المحددة"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/lowcodesaveoptionsproviderofplaceholders/
---
## LowCodeSaveOptionsProviderOfPlaceHolders constructor

ينشئ نسخة لتوفير خيارات الحفظ وفقًا للقوالب المحددة.

```csharp
public LowCodeSaveOptionsProviderOfPlaceHolders(string pathTemplate)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| pathTemplate | String | قالب مسار الملف الناتج. |

### ملاحظات

العناصر النائبة المدعومة في قالب مسار الملف: ${SheetIndex}: سيتم استبداله برقم ورقة الجزء المقسوم${SheetName}: سيتم استبداله باسم ورقة الجزء المقسوم${SplitPartIndex}: سيتم استبداله برقم الجزء المقسوم${SheetIndexPrefix}: سيتم استبداله بـ [`SheetIndexPrefix`](../sheetindexprefix/)${SheetNamePrefix}: سيتم استبداله بـ [`SheetNamePrefix`](../sheetnameprefix/)${SplitPartPrefix}: سيتم استبداله بـ [`SplitPartPrefix`](../splitpartprefix/)

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersMethodCtorWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // استدعاء طريقة #ctor مع معامل String
                string pathTemplate = "output_{sheet}_part_{part}.xlsx";
                var provider = new LowCodeSaveOptionsProviderOfPlaceHolders(pathTemplate);

                // تعيين بعض الخصائص
                provider.SheetIndexOffset = 0;
                provider.SplitPartIndexOffset = 0;
                provider.SheetNamePrefix = "Sheet_";
                provider.SplitPartPrefix = "Part_";

                Console.WriteLine("LowCodeSaveOptionsProviderOfPlaceHolders created successfully with path template: " + pathTemplate);
                Console.WriteLine($"SheetNamePrefix: {provider.SheetNamePrefix}, SplitPartPrefix: {provider.SplitPartPrefix}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating LowCodeSaveOptionsProviderOfPlaceHolders: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("LowCodeSaveOptionsProviderDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


