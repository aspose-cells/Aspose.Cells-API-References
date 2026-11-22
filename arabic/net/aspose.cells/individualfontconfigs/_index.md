---
title: "الفئة IndividualFontConfigs"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.IndividualFontConfigs. إعدادات الخط لكل كائن Workbook."
type: docs
url: /ar/net/aspose.cells/individualfontconfigs/
---
## IndividualFontConfigs class

إعدادات الخط لكل كائن [`Workbook`](../workbook/) .

```csharp
public class IndividualFontConfigs
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [IndividualFontConfigs](individualfontconfigs/)() | منشئ. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [GetFontSources](../../aspose.cells/individualfontconfigs/getfontsources/)() | يحصل على نسخة من المصفوفة التي تحتوي على قائمة المصادر. |
| [GetFontSubstitutes](../../aspose.cells/individualfontconfigs/getfontsubstitutes/)(string) | يعيد مصفوفة تحتوي على أسماء بدائل الخط لاستخدامها إذا لم يتوفر الخط الأصلي. |
| [SetFontFolder](../../aspose.cells/individualfontconfigs/setfontfolder/)(string, bool) | يعيّن مجلد الخطوط |
| [SetFontFolders](../../aspose.cells/individualfontconfigs/setfontfolders/)(string[], bool) | يضبط مجلدات الخطوط |
| [SetFontSources](../../aspose.cells/individualfontconfigs/setfontsources/)(FontSourceBase[]) | يعيّن مصادر الخط. |
| [SetFontSubstitutes](../../aspose.cells/individualfontconfigs/setfontsubstitutes/)(string, string[]) | يضبط أسماء بدائل الخط لاسم خط أصلي معين. |

### أمثلة

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassIndividualFontConfigsDemo
    {
        public static void Run()
        {
            // إنشاء أدلة مؤقتة لمصادر الخطوط
            string tempFontFolder1 = Path.Combine(Path.GetTempPath(), "FontFolder1_" + Guid.NewGuid().ToString());
            string tempFontFolder2 = Path.Combine(Path.GetTempPath(), "FontFolder2_" + Guid.NewGuid().ToString());
            Directory.CreateDirectory(tempFontFolder1);
            Directory.CreateDirectory(tempFontFolder2);

            // إنشاء ملف CSV تجريبي
            string csvFilePath = "sample_data.csv";
            File.WriteAllText(csvFilePath, "Name,Age\nJohn,30\nAlice,25", Encoding.UTF8);

            try
            {
                // تهيئة تكوين الخط
                IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

                // تعيين بدائل الخط لـ Arial
                fontConfigs.SetFontSubstitutes("Arial", new string[] { "Times New Roman", "Verdana" });

                // تكوين أدلة الخطوط
                fontConfigs.SetFontFolder(tempFontFolder1, false);
                fontConfigs.SetFontFolders(new string[] { tempFontFolder1, tempFontFolder2 }, true);

                // تكوين مصادر الخطوط
                FontSourceBase[] fontSources = {
                    new FolderFontSource(tempFontFolder1, false),
                    new FolderFontSource(tempFontFolder2, true)
                };
                fontConfigs.SetFontSources(fontSources);

                // إنشاء خيارات تحميل النص مع تكوينات الخط
                TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
                {
                    FontConfigs = fontConfigs
                };

                // تحميل المصنف باستخدام الخيارات المُكوَّنة
                using (Workbook workbook = new Workbook(csvFilePath, loadOptions))
                {
                    // حفظ كملف Excel
                    workbook.Save("output_with_font_config.xlsx");
                }
            }
            finally
            {
                // تنظيف الموارد المؤقتة
                if (Directory.Exists(tempFontFolder1)) Directory.Delete(tempFontFolder1, true);
                if (Directory.Exists(tempFontFolder2)) Directory.Delete(tempFontFolder2, true);
                if (File.Exists(csvFilePath)) File.Delete(csvFilePath);
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


