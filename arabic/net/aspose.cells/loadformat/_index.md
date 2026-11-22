---
title: "تعداد LoadFormat"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.LoadFormat. يمثل تنسيق ملف التحميل"
type: docs
url: /ar/net/aspose.cells/loadformat/
---
## LoadFormat enumeration

يمثل تنسيق ملف التحميل.

```csharp
public enum LoadFormat
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Auto | `0` | يمثل التعرف على التنسيق تلقائيًا. |
| Csv | `1` | ملف نصي قيم مفصولة بفواصل (CSV). |
| CSV | `1` | ملف نصي قيم مفصولة بفواصل (CSV). ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية Csv. سيتم إزالة هذه الخاصية بعد 6 أشهر منذ أبريل 2021. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته. |
| Xlsx | `6` | يمثل دفتر عمل أو قالب Office Open XML spreadsheetML، مع أو بدون وحدات ماكرو. |
| Tsv | `11` | ملف نصي قيم مفصولة بجدولة (TSV). |
| TSV | `11` | ملف نصي قيم مفصولة بجدولة (TSV). ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية Tsv. سيتم إزالة هذه الخاصية بعد 6 أشهر منذ أبريل 2021. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته. |
| TabDelimited | `11` | يمثل ملف نصي مفصول بجدولة، وهو نفسه Tsv. |
| Html | `12` | يمثل ملف html. |
| MHtml | `13` | يمثل ملف mhtml. |
| Ods | `14` | ملف Open Document Sheet (ODS). |
| ODS | `14` | ملف Open Document Sheet (ODS). ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية Ods. سيتم إزالة هذه الخاصية بعد 6 أشهر منذ أبريل 2021. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته. |
| Excel97To2003 | `5` | يمثل ملف Excel97-2003 xls. |
| SpreadsheetML | `15` | يمثل ملف Excel 2003 xml. |
| Xlsb | `16` | يمثل ملف xlsb. |
| Ots | `31` | ملف Open Document Template Sheet (OTS). |
| Numbers | `56` | يمثل ملف numbers. |
| Fods | `59` | يمثل تنسيق ملف OpenDocument Flat XML Spreadsheet (.fods). |
| FODS | `59` | يمثل تنسيق ملف OpenDocument Flat XML Spreadsheet (.fods). ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية Fods. سيتم إزالة هذه الخاصية بعد 6 أشهر منذ أبريل 2021. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته. |
| Sxc | `60` | يمثل تنسيق ملف StarOffice Calc Spreadsheet (.sxc). |
| SXC | `60` | يمثل تنسيق ملف StarOffice Calc Spreadsheet (.sxc). ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية Sxc. سيتم إزالة هذه الخاصية بعد 6 أشهر منذ أبريل 2021. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته. |
| Xml | `51` | يمثل ملف xml بسيط. |
| Epub | `52` | يمثل ملف EPUB. |
| Azw3 | `53` | يمثل ملف AZW3. |
| Chm | `54` | يمثل ملف CHM. |
| Markdown | `55` | يمثل ملف Markdown. |
| Unknown | `255` | يمثل تنسيقًا غير معروف، لا يمكن تحميله. |
| Image | `254` | صورة |
| Json | `513` | Json |
| Dif | `30` | تنسيق تبادل البيانات. |
| Dbf | `515` | ملف بيانات Xbase |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFormatDemo
    {
        public static void LoadFormatExample()
        {
            // تحميل ملف Excel بصيغ مختلفة باستخدام Aspose.Cells
            string[] filePaths = {
                "LoadFormatDemo_original.xlsx",
                "LoadFormatDemo_original.xls",
                "LoadFormatDemo_original.csv",
                "LoadFormatDemo_original.json"
            };

            foreach (var filePath in filePaths)
            {
                // تحديد صيغة التحميل بناءً على امتداد الملف
                LoadFormat loadFormat = GetLoadFormat(filePath);

                // إنشاء LoadOptions مع صيغة التحميل المحددة
                LoadOptions loadOptions = new LoadOptions(loadFormat);

                // تحميل دفتر العمل باستخدام خيارات التحميل المحددة
                Workbook workbook = new Workbook(filePath, loadOptions);

                // إجراء بعض العمليات على دفتر العمل
                Console.WriteLine($"Loaded file: {filePath}");
                Console.WriteLine($"Number of sheets: {workbook.Worksheets.Count}");

                // حفظ دفتر العمل إلى ملف جديد
                string outputFilePath = $"output_{System.IO.Path.GetFileName(filePath)}";
                workbook.Save(outputFilePath);
                Console.WriteLine($"Saved file as: {outputFilePath}");
            }
        }

        private static LoadFormat GetLoadFormat(string filePath)
        {
            string extension = System.IO.Path.GetExtension(filePath).ToLower();
            switch (extension)
            {
                case ".xlsx":
                    return LoadFormat.Xlsx;
                case ".xls":
                    return LoadFormat.Excel97To2003;
                case ".csv":
                    return LoadFormat.Csv;
                case ".json":
                    return LoadFormat.Json;
                default:
                    return LoadFormat.Auto;
            }
        }
    }

}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


