---
title: "TextBoxCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextBoxCollection. تحصل على عنصر TextBox في الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells.drawing/textboxcollection/item/
---
## TextBoxCollection indexer (1 of 2)

يحصل على عنصر [`TextBox`](../../textbox/) في الفهرس المحدد.

```csharp
public TextBox this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس الذي يبدأ من الصفر للعنصر. |

### قيمة الإرجاع

العنصر عند الفهرس المحدد.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض صناديق النص إلى ورقة العمل
            int textBoxIndex1 = worksheet.TextBoxes.Add(10, 10, 100, 50);
            TextBox textBox1 = worksheet.TextBoxes[textBoxIndex1];
            textBox1.Text = "TextBox 1";
            
            int textBoxIndex2 = worksheet.TextBoxes.Add(10, 70, 100, 50);
            TextBox textBox2 = worksheet.TextBoxes[textBoxIndex2];
            textBox2.Text = "TextBox 2";

            // الوصول إلى صناديق النص باستخدام خاصية Item
            TextBoxCollection textBoxCollection = worksheet.TextBoxes;
            int index = textBoxCollection.Count - 1;
            TextBox lastTextBox = textBoxCollection[index];

            // إخراج نص آخر صندوق نص
            Console.WriteLine("Last TextBox Text: " + lastTextBox.Text);
        }
    }
}
```

### انظر أيضًا

* class [TextBox](../../textbox/)
* class [TextBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## TextBoxCollection indexer (2 of 2)

يحصل على عنصر [`TextBox`](../../textbox/) بالاسم.

```csharp
public TextBox this[string name] { get; }
```

| معامل | الوصف |
| --- | --- |
| name | اسم صندوق النص. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف صناديق النص إلى ورقة العمل واحصل على مؤشراتهم
            int textBoxIndex1 = worksheet.TextBoxes.Add(10, 10, 100, 50);
            TextBox textBox1 = worksheet.TextBoxes[textBoxIndex1];
            textBox1.Name = "textbox 1";
            textBox1.Text = "First TextBox";

            int textBoxIndex2 = worksheet.TextBoxes.Add(10, 70, 100, 50);
            TextBox textBox2 = worksheet.TextBoxes[textBoxIndex2];
            textBox2.Name = "textbox 2";
            textBox2.Text = "Second TextBox";

            // الوصول إلى صندوق النص باستخدام خاصية Item بالاسم
            string txtboxName = "textbox 1";
            TextBox txb2 = worksheet.TextBoxes[txtboxName];
            if (txb2 != null)
            {
                Console.WriteLine("Found TextBox: " + txb2.Name);
                Console.WriteLine("TextBox Text: " + txb2.Text);
            }
        }
    }
}
```

### انظر أيضًا

* class [TextBox](../../textbox/)
* class [TextBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


