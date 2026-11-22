---
title: "الفئة ConversionUtility"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Utility.ConversionUtility. تمثل أداة لتحويل الملفات إلى صيغ أخرى"
type: docs
url: /ar/net/aspose.cells.utility/conversionutility/
---
## ConversionUtility class

يمثل أداة لتحويل الملفات إلى صيغ أخرى.

```csharp
public class ConversionUtility
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| static [Convert](../../aspose.cells.utility/conversionutility/convert/#convert_1)(string, string) | يقوم بتحويل ملفات Excel إلى صيغ أخرى. |
| static [Convert](../../aspose.cells.utility/conversionutility/convert/#convert)(string, LoadOptions, string, SaveOptions) | يقوم بتحويل ملفات Excel إلى صيغ أخرى. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;
    using System.IO;

    public class UtilityClassConversionUtilityDemo
    {
        public static void Run()
        {
            // إنشاء ملف CSV نموذجي للتحويل
            string sourceFile = "sample.csv";
            string outputFile = "converted.xlsx";

            try
            {
                // إنشاء محتوى CSV نموذجي
                File.WriteAllText(sourceFile, "Product,Price,Quantity\nApple,1.50,100\nBanana,0.75,150\nOrange,1.25,120");

                // تحويل CSV إلى XLSX باستخدام طريقة تحويل ثابتة
                ConversionUtility.Convert(sourceFile, outputFile);

                Console.WriteLine($"Successfully converted {sourceFile} to {outputFile}");

                // تحقق من التحويل عن طريق فحص ما إذا كان ملف الإخراج موجودًا
                if (File.Exists(outputFile))
                {
                    Console.WriteLine("Output file created successfully");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during conversion: {ex.Message}");
            }
            finally
            {
                // تنظيف الملفات المؤقتة
                if (File.Exists(sourceFile))
                {
                    File.Delete(sourceFile);
                }
                if (File.Exists(outputFile))
                {
                    File.Delete(outputFile);
                }
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


