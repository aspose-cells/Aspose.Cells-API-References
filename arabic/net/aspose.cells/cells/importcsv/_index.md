---
title: "Cells.ImportCSV"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. استيراد ملف CSV إلى الخلايا"
type: docs
url: /ar/net/aspose.cells/cells/importcsv/
---
## ImportCSV(string, string, bool, int, int) {#importcsv_3}

استيراد ملف CSV إلى الخلايا.

```csharp
public void ImportCSV(string fileName, string splitter, bool convertNumericData, int firstRow, 
    int firstColumn)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | String | اسم ملف CSV. |
| المقسم | String | المقسم |
| convertNumericData | منطقي | ما إذا كان النص في ملف النص يتم تحويله إلى بيانات رقمية. |
| firstRow | Int32 | رقم الصف للخلية الأولى التي سيتم الاستيراد فيها. |
| firstColumn | Int32 | رقم العمود للخلية الأولى التي سيتم الاستيراد فيها. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportCSVWithStringStringBooleanInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // المسار إلى ملف CSV
            string csvPath = "example.csv";
            
            // استيراد بيانات CSV بدءًا من الخلية A1 (الصف 0، العمود 0)
            // استخدام الفاصلة المنقوطة كفاصل وتحويل البيانات الرقمية
            cells.ImportCSV(csvPath, ";", true, 0, 0);

            // احفظ المصنف
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportCSV(Stream, string, bool, int, int) {#importcsv_1}

استيراد ملف CSV إلى الخلايا.

```csharp
public void ImportCSV(Stream stream, string splitter, bool convertNumericData, int firstRow, 
    int firstColumn)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | Stream | تدفق ملف CSV. |
| المقسم | String | المقسم |
| convertNumericData | منطقي | ما إذا كان النص في ملف النص يتم تحويله إلى بيانات رقمية. |
| firstRow | Int32 | رقم الصف للخلية الأولى التي سيتم الاستيراد فيها. |
| firstColumn | Int32 | رقم العمود للخلية الأولى التي سيتم الاستيراد فيها. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsMethodImportCSVWithStreamStringBooleanInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // إنشاء بيانات CSV تجريبية في الذاكرة
            string csvData = "Name,Age,City\nJohn,30,New York\nAlice,25,London\nBob,35,Paris";
            byte[] byteArray = System.Text.Encoding.UTF8.GetBytes(csvData);
            MemoryStream csvStream = new MemoryStream(byteArray);

            try
            {
                // استدعاء طريقة ImportCSV مع معلمات Stream، String، Boolean، Int32، Int32
                cells.ImportCSV(csvStream, ",", true, 0, 0);

                Console.WriteLine("CSV data imported successfully to worksheet.");
                Console.WriteLine($"Data range: A1 to {cells.MaxDisplayRange}");

                // احفظ المصنف
                workbook.Save("ImportCSVFromStreamDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing CSV: {ex.Message}");
            }
            finally
            {
                csvStream?.Dispose();
            }
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportCSV(string, TxtLoadOptions, int, int) {#importcsv_2}

استيراد ملف CSV إلى الخلايا.

```csharp
public void ImportCSV(string fileName, TxtLoadOptions options, int firstRow, int firstColumn)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | String | اسم ملف CSV. |
| خيارات | TxtLoadOptions | خيارات التحميل لقراءة ملف النص |
| firstRow | Int32 | رقم الصف للخلية الأولى التي سيتم الاستيراد فيها. |
| firstColumn | Int32 | رقم العمود للخلية الأولى التي سيتم الاستيراد فيها. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportCSVWithStringTxtLoadOptionsInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء خيارات تحميل CSV
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.Separator = ',';
            loadOptions.ConvertDateTimeData = true;
            loadOptions.ConvertNumericData = true;
            loadOptions.ParsingFormulaOnOpen = true;

            // مسار ملف CSV النموذجي (استبدله بالمسار الفعلي في بيئتك)
            string csvFilePath = "example.csv";
            
            // استيراد بيانات CSV بدءًا من الخلية A1 (الصف 0، العمود 0)
            worksheet.Cells.ImportCSV(csvFilePath, loadOptions, 0, 0);

            // احفظ المصنف
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [TxtLoadOptions](../../txtloadoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportCSV(Stream, TxtLoadOptions, int, int) {#importcsv}

استيراد ملف CSV إلى الخلايا.

```csharp
public void ImportCSV(Stream stream, TxtLoadOptions options, int firstRow, int firstColumn)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | Stream | تدفق ملف CSV. |
| خيارات | TxtLoadOptions | خيارات التحميل لقراءة ملف النص |
| firstRow | Int32 | رقم الصف للخلية الأولى التي سيتم الاستيراد فيها. |
| firstColumn | Int32 | رقم العمود للخلية الأولى التي سيتم الاستيراد فيها. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsMethodImportCSVWithStreamTxtLoadOptionsInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // احصل على مجموعة Cells
            Cells cells = worksheet.Cells;

            // إنشاء بيانات CSV نموذجية
            string csvData = "Name,Age,City\nJohn,30,New York\nJane,25,Los Angeles\nBob,35,Chicago";

            // إنشاء تدفق ذاكرة يحتوي على بيانات CSV
            MemoryStream csvStream = new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData));

            try
            {
                // إنشاء TxtLoadOptions لاستيراد CSV
                TxtLoadOptions loadOptions = new TxtLoadOptions();
                loadOptions.Separator = ',';
                loadOptions.ConvertNumericData = true;

                // استيراد بيانات CSV بدءًا من الصف 0، العمود 0
                cells.ImportCSV(csvStream, loadOptions, 0, 0);

                // احفظ المصنف
                workbook.Save("ImportCSVDemo.xlsx");

                Console.WriteLine("CSV data imported successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing CSV: {ex.Message}");
            }
            finally
            {
                // تحرير التدفق
                csvStream.Dispose();
            }
        }
    }
}
```

### انظر أيضًا

* class [TxtLoadOptions](../../txtloadoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


