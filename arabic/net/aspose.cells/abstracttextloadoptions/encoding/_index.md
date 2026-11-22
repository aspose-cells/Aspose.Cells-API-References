---
title: "AbstractTextLoadOptions.Encoding"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية AbstractTextLoadOptions. تحصل وتعيّن الترميز الافتراضي. ينطبق فقط على ملفات csv"
type: docs
url: /ar/net/aspose.cells/abstracttextloadoptions/encoding/
---
## AbstractTextLoadOptions.Encoding property

يحصل ويعيّن الترميز الافتراضي. ينطبق فقط على ملفات csv.

```csharp
public Encoding Encoding { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AbstractTextLoadOptionsPropertyEncodingDemo
    {
        public static void Run()
        {
            // إنشاء بيانات CSV نموذجية بترميز ASCII
            MemoryStream ms = new MemoryStream();
            byte[] data = Encoding.ASCII.GetBytes("Name,Age\nJohn,30\nJane,25");
            ms.Write(data, 0, data.Length);
            ms.Seek(0, SeekOrigin.Begin);

            // تحميل دفتر العمل مع تحديد ترميز ASCII
            Workbook wb = new Workbook(ms, new TxtLoadOptions() { Encoding = Encoding.ASCII });
            Cells cells = wb.Worksheets[0].Cells;

            // عرض البيانات المحملة
            Console.WriteLine($"A1: {cells[0, 0].StringValue}");
            Console.WriteLine($"B1: {cells[0, 1].StringValue}");
            Console.WriteLine($"A2: {cells[1, 0].StringValue}");
            Console.WriteLine($"B2: {cells[1, 1].IntValue}");

            // إضافة بعض النصوص Unicode
            cells[2, 0].PutValue("日本語のテキスト");
            
            // احفظ باستخدام ترميز UTF-8
            MemoryStream outputStream = new MemoryStream();
            wb.Save(outputStream, new TxtSaveOptions() { Encoding = Encoding.UTF8 });
            
            // اعرض أول بضعة بايت لإظهار BOM الخاص بـ UTF-8
            byte[] outputBytes = outputStream.ToArray();
            Console.WriteLine($"First 3 bytes: {BitConverter.ToString(outputBytes, 0, 3)}");
        }
    }
}
```

### انظر أيضًا

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


