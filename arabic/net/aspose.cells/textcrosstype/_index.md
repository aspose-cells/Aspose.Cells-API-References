---
title: "التعداد TextCrossType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.TextCrossType. يعدد نوع عرض النص عندما يكون عرض النص أكبر من عرض الخلية"
type: docs
url: /ar/net/aspose.cells/textcrosstype/
---
## TextCrossType enumeration

يسرد نوع عرض النص عندما يكون عرض النص أكبر من عرض الخلية.

```csharp
public enum TextCrossType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Default | `1` | عرض النص كما في Microsoft Excel. |
| CrossKeep | `2` | عرض كل النص عبر عبور خلايا أخرى والاحتفاظ بنص الخلايا المتقاطعّة. |
| CrossOverride | `3` | اعرض كل النص عن طريق عبور الخلايا الأخرى وتجاوز نص الخلايا المتقاطعة. |
| StrictInCell | `4` | اعرض النص فقط ضمن عرض الخلية. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class CellsClassTextCrossTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // قم بتعيين نص تجريبي في خلية قد يحدث فيها تجاوز.
            worksheet.Cells["A1"].PutValue("This is a long text that might overflow the cell");
            
            // إنشاء خيارات الصورة أو الطباعة
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // عرض إعدادات مختلفة لـ TextCrossType
            options.TextCrossType = TextCrossType.Default;
            SaveToImage(workbook, options, "TextCrossType_Default.png");
            
            options.TextCrossType = TextCrossType.CrossKeep;
            SaveToImage(workbook, options, "TextCrossType_CrossKeep.png");
            
            options.TextCrossType = TextCrossType.CrossOverride;
            SaveToImage(workbook, options, "TextCrossType_CrossOverride.png");
            
            options.TextCrossType = TextCrossType.StrictInCell;
            SaveToImage(workbook, options, "TextCrossType_StrictInCell.png");
        }
        
        private static void SaveToImage(Workbook workbook, ImageOrPrintOptions options, string fileName)
        {
            SheetRender sr = new SheetRender(workbook.Worksheets[0], options);
            sr.ToImage(0, fileName);
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


