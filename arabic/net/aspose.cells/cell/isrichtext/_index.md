---
title: "Cell.IsRichText"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cell. تشير إلى ما إذا كانت القيمة النصية لهذه الخلية نصًا منسقًا غنيًا"
type: docs
url: /ar/net/aspose.cells/cell/isrichtext/
---
## Cell.IsRichText method

يشير إلى ما إذا كانت قيمة السلسلة لهذه الخلية نصًا منسقًا بنص غني.

```csharp
public bool IsRichText()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodIsRichTextDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء خلية بتنسيق نص غني
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Hello World");
            
            // تطبيق تنسيق نص غني
            FontSetting boldFont = cell.GetCharacters()[0];
            boldFont.Font.IsBold = true;
            
            FontSetting normalFont = cell.GetCharacters()[6];
            normalFont.Font.IsBold = false;
            
            // تحقق مما إذا كانت الخلية تحتوي على نص غني
            bool isRichText = cell.IsRichText();
            Console.WriteLine("Is cell A1 rich text? " + isRichText);
            
            // احفظ المصنف
            workbook.Save("RichTextDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


