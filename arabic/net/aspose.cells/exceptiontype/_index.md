---
title: "التعداد ExceptionType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.ExceptionType. يمثل رمز نوع استثناء مخصص"
type: docs
url: /ar/net/aspose.cells/exceptiontype/
---
## ExceptionType enumeration

يمثل رمز نوع الاستثناء المخصص.

```csharp
public enum ExceptionType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Chart | `0` | إعداد مخطط غير صالح. |
| DataType | `1` | إعداد نوع بيانات غير صالح. |
| DataValidation | `2` | إعداد تحقق من البيانات غير صالح. |
| ConditionalFormatting | `3` | إعداد تحقق من البيانات غير صالح. |
| FileFormat | `4` | تنسيق ملف غير صالح. |
| Formula | `5` | صيغة غير صالحة. |
| InvalidData | `6` | بيانات غير صالحة. |
| InvalidOperator | `7` | عامل غير صالح. |
| IncorrectPassword | `8` | كلمة مرور غير صحيحة. |
| License | `9` | أخطاء متعلقة بالترخيص. |
| Limitation | `10` | خطأ تجاوز حدود مايكروسوفت إكسل. |
| PageSetup | `11` | إعداد تخطيط الصفحة غير صالح. |
| PivotTable | `12` | إعداد PivotTable غير صالح. |
| Shape | `13` | إعداد كائن الرسم غير صالح. |
| Sparkline | `14` | إعداد كائن Sparkline غير صالح. |
| SheetName | `15` | اسم ورقة العمل غير صالح. |
| SheetType | `16` | نوع ورقة العمل غير صالح. |
| Interrupted | `17` | تم إيقاف العملية. |
| IO | `18` | الملف غير صالح. |
| Permission | `19` | يتطلب الإذن لفتح هذا الملف. |
| UnsupportedFeature | `20` | ميزة غير مدعومة. |
| UnsupportedStream | `21` | تدفق غير مدعوم للفتح. |
| UndisclosedInformation | `22` | الملفات تحتوي على بعض المعلومات غير المكشوفة. |
| FileCorrupted | `23` | محتوى الملف تالف. |
| DefinedName | `25` | اسم معرف غير صالح |
| Font | `26` | خط غير صالح |
| AutoFilter | `27` | إعداد الفلتر التلقائي غير صالح. |
| FontSubstitution | `28` | نوع تحذير استبدال الخط عندما لا يتم العثور على الخط، يمكن الحصول على هذا النوع من التحذير. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExceptionTypeDemo
    {
        public static void ExceptionTypeExample()
        {
            try
            {
                // إنشاء دفتر عمل جديد
                Workbook workbook = new Workbook();

                // محاولة تعيين اسم ورقة عمل غير صالح لتوليد استثناء.
                workbook.Worksheets[0].Name = "Invalid/Name";

                // احفظ المصنف
                workbook.Save("ExceptionTypeExample.xlsx");
            }
            catch (CellsException ex)
            {
                // معالجة CellsException
                Console.WriteLine("An error occurred: " + ex.Message);
                Console.WriteLine("Exception Type Code: " + ex.Code);
                
                // تحقق من نوع الاستثناء
                switch (ex.Code)
                {
                    case ExceptionType.SheetName:
                        Console.WriteLine("The worksheet name is invalid.");
                        break;
                    case ExceptionType.FileFormat:
                        Console.WriteLine("The file format is invalid.");
                        break;
                    // أضف المزيد من الحالات حسب الحاجة لأنواع الاستثناء المختلفة
                    default:
                        Console.WriteLine("An unknown error occurred.");
                        break;
                }
            }
            catch (Exception ex)
            {
                // معالجة أي استثناءات أخرى
                Console.WriteLine("An unexpected error occurred: " + ex.Message);
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


