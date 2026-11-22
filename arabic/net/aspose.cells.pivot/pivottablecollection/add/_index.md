---
title: "PivotTableCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotTableCollection. تضيف PivotTable حديث جديد منذ Excel 2007 في الصف والعمود المحددين في ورقة العمل مع الخيارات الافتراضية"
type: docs
url: /ar/net/aspose.cells.pivot/pivottablecollection/add/
---
## Add(string, string) {#add_2}

يضيف PivotTable حديث جديد (منذ Excel 2007) في صف وعمود ورقة العمل المحددة مع الخيارات الافتراضية.

```csharp
public PivotTable Add(string sourceData, string cellName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceData | String | نطاق خلايا البيانات للـ PivotTable الجديد. مثال: Sheet1!A1:C8 |
| cellName | String | اسم الخلية الموجودة في الزاوية العلوية اليسرى لوجهة الـ PivotTable. |

### قيمة الإرجاع

مثيل الـ PivotTable الذي تم إنشاؤه حديثًا.

### انظر أيضًا

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, PivotTableCreateOptions) {#add_3}

يضيف PivotTable حديث جديد (منذ Excel 2007) في صف وعمود ورقة العمل المحددة مع الخيارات الافتراضية.

```csharp
public PivotTable Add(string sourceData, string cellName, PivotTableCreateOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceData | String | نطاق خلايا البيانات للـ PivotTable الجديد. مثال: Sheet1!A1:C8 |
| cellName | String | اسم الخلية الموجودة في الزاوية العلوية اليسرى لوجهة الـ PivotTable. |
| خيارات | PivotTableCreateOptions | خيارات إنشاء جدول محوري. |

### قيمة الإرجاع

مثيل الـ PivotTable الذي تم إنشاؤه حديثًا.

### انظر أيضًا

* class [PivotTable](../../pivottable/)
* class [PivotTableCreateOptions](../../pivottablecreateoptions/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int) {#add}

يضيف PivotTable حديث جديد (منذ Excel 2007) في صف وعمود ورقة العمل المحددة مع الخيارات الافتراضية.

```csharp
public PivotTable Add(string sourceData, int row, int column)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceData | String | نطاق خلايا البيانات للـ PivotTable الجديد. مثال: Sheet1!A1:C8 |
| صف | Int32 | فهرس الصف الصفري للزاوية العلوية اليسرى لوجهة الـ PivotTable. |
| عمود | Int32 | فهرس العمود الصفري للزاوية العلوية اليسرى لوجهة الـ PivotTable. |

### قيمة الإرجاع

مثيل الـ PivotTable الذي تم إنشاؤه حديثًا.

### انظر أيضًا

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, PivotTableCreateOptions) {#add_1}

يضيف PivotTable جديد في صف وعمود ورقة العمل المحددة.

```csharp
public PivotTable Add(string sourceData, int row, int column, PivotTableCreateOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceData | String | نطاق خلايا البيانات للـ PivotTable الجديد. مثال: Sheet1!A1:C8 |
| صف | Int32 | فهرس الصف الصفري للزاوية العلوية اليسرى لوجهة الـ PivotTable. |
| عمود | Int32 | فهرس العمود الصفري للزاوية العلوية اليسرى لوجهة الـ PivotTable. |
| خيارات | PivotTableCreateOptions | خيارات إنشاء PivotTable. |

### قيمة الإرجاع

مثيل الـ PivotTable الذي تم إنشاؤه حديثًا.

### انظر أيضًا

* class [PivotTable](../../pivottable/)
* class [PivotTableCreateOptions](../../pivottablecreateoptions/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string) {#add_9}

يضيف PivotTable جديدًا بتخطيط ونمط Excel 97-2003 القديم.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, string destCellName, string tableName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceData | String | البيانات لذاكرة التخزين المؤقت لـ PivotTable الجديد. |
| destCellName | String | الخلية في الزاوية العلوية اليسرى لنطاق الوجهة لتقرير PivotTable. |
| tableName | String | اسم تقرير PivotTable الجديد. |

### قيمة الإرجاع

الفهرس في قائمة PivotTable هذه.

### ملاحظات

ملاحظة: هذه الطريقة قديمة. إنها تعادل استدعاء PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) مع `NewPivotTableOptions.IsXlsClassic = true`. يرجى استخدام نسخة PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا من سبتمبر 2026. نعتذر عن أي إزعاج.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodAddWithStringStringStringDemo
    {
        public static void Run()
        {
            // إنشاء مصنف من CSV المصدر
            Workbook workbook = new Workbook();
            Worksheet sourceSheet = workbook.Worksheets[0];
            sourceSheet.Name = "SourceData";
            
            // أضف بيانات تجريبية
            sourceSheet.Cells["A1"].PutValue("Category");
            sourceSheet.Cells["B1"].PutValue("Value");
            sourceSheet.Cells["A2"].PutValue("A");
            sourceSheet.Cells["B2"].PutValue(10);
            sourceSheet.Cells["A3"].PutValue("B");
            sourceSheet.Cells["B3"].PutValue(20);
            sourceSheet.Cells["A4"].PutValue("A");
            sourceSheet.Cells["B4"].PutValue(30);

            // إنشاء ورقة عمل جدول محوري
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            
            // احصل على نطاق البيانات المصدر
            Aspose.Cells.Range sourceRange = sourceSheet.Cells.MaxDisplayRange;
            string sourceData = String.Format("=SourceData!{0}", sourceRange.Address);
            
            // إضافة PivotTable باستخدام معلمات String, String, String
            PivotTableCollection pivotTables = pivotSheet.PivotTables;
            int pivotIndex = pivotTables.Add(sourceData, "A1", "MyPivotTable");
            
            // تكوين جدول محوري
            PivotTable pivotTable = pivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // احفظ المصنف
            workbook.Save("PivotTableDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string, bool) {#add_10}

يضيف PivotTable جديدًا بتخطيط ونمط Excel 97-2003 القديم.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, string, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, string destCellName, string tableName, bool useSameSource)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceData | String | البيانات لذاكرة التخزين المؤقت لـ PivotTable الجديد. |
| destCellName | String | الخلية في الزاوية العلوية اليسرى لنطاق الوجهة لتقرير PivotTable. |
| tableName | String | اسم تقرير PivotTable الجديد. |
| useSameSource | منطقي | يشير إلى ما إذا كان يتم استخدام نفس مصدر البيانات عندما يكون جدول محوري آخر موجود قد استخدم هذا المصدر. إذا كانت الخاصية true، فستوفر الذاكرة. |

### قيمة الإرجاع

فهرس المخزن المضاف حديثًا.

### ملاحظات

ملاحظة: هذه الطريقة قديمة. إنها تعادل استدعاء PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) مع `NewPivotTableOptions.IsXlsClassic = true`. يرجى استخدام نسخة PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا من سبتمبر 2026. نعتذر عن أي إزعاج.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringStringStringBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // تحديد معلمات طريقة Add
            string sourceData = "A1:B4";
            string destCellName = "E5";
            string tableName = "FruitPivotTable";
            bool useSameSource = true;

            try
            {
                // استدعاء طريقة Add مع المعلمات (String, String, String, Boolean)
                int index = worksheet.PivotTables.Add(sourceData, destCellName, tableName, useSameSource);
                
                Console.WriteLine($"Pivot table added successfully at index: {index}");
                Console.WriteLine($"Pivot table name: {worksheet.PivotTables[index].Name}");
                Console.WriteLine($"Pivot table location: {worksheet.PivotTables[index].TableRange1}");

                // تكوين جدول المحور
                PivotTable pivotTable = worksheet.PivotTables[index];
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // احفظ المصنف
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, string) {#add_6}

يضيف PivotTable جديدًا بتخطيط ونمط Excel 97-2003 القديم.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, int row, int column, string tableName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceData | String | نطاق خلايا البيانات للـ PivotTable الجديد. مثال : Sheet1!A1:C8 |
| صف | Int32 | فهرس الصف للخلية في الزاوية العلوية اليسرى لنطاق الوجهة لتقرير PivotTable. |
| عمود | Int32 | فهرس العمود للخلية في الزاوية العلوية اليسرى لنطاق الوجهة لتقرير PivotTable. |
| tableName | String | اسم تقرير PivotTable الجديد. |

### قيمة الإرجاع

الفهرس في قائمة PivotTable هذه.

### ملاحظات

ملاحظة: هذه الطريقة قديمة. إنها تعادل استدعاء PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) مع `NewPivotTableOptions.IsXlsClassic = true`. يرجى استخدام نسخة PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا من سبتمبر 2026. نعتذر عن أي إزعاج.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodAddWithStringInt32Int32StringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة ورقة عمل للبيانات
            Worksheet dataWorksheet = workbook.Worksheets[0];
            dataWorksheet.Name = "Data";
            
            // أضف بيانات تجريبية
            dataWorksheet.Cells["A1"].PutValue("Category");
            dataWorksheet.Cells["B1"].PutValue("Product");
            dataWorksheet.Cells["C1"].PutValue("Sales");
            
            dataWorksheet.Cells["A2"].PutValue("Electronics");
            dataWorksheet.Cells["B2"].PutValue("Laptop");
            dataWorksheet.Cells["C2"].PutValue(1000);
            
            dataWorksheet.Cells["A3"].PutValue("Electronics");
            dataWorksheet.Cells["B3"].PutValue("Phone");
            dataWorksheet.Cells["C3"].PutValue(800);
            
            dataWorksheet.Cells["A4"].PutValue("Furniture");
            dataWorksheet.Cells["B4"].PutValue("Chair");
            dataWorksheet.Cells["C4"].PutValue(200);
            
            // إضافة ورقة عمل للـ PivotTable
            Worksheet pivotWorksheet = workbook.Worksheets.Add("PivotTable");
            
            // إضافة PivotTable باستخدام طريقة Add مع معلمات (String, Int32, Int32, String)
            string pivotDataRange = "Data!A1:C4";
            int row = 0;
            int column = 0;
            string tableName = "SalesPivotTable";
            
            int pivotIndex = pivotWorksheet.PivotTables.Add(pivotDataRange, row, column, tableName);
            
            // الوصول إلى PivotTable
            PivotTable pivotTable = pivotWorksheet.PivotTables[pivotIndex];
            
            // إضافة حقول إلى الجدول المحوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // تعيين دالة التجميع
            pivotTable.DataFields[0].Function = ConsolidationFunction.Sum;
            
            // تحديث وحساب بيانات جدول البيفوت
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // احفظ المصنف
            workbook.Save("PivotTableDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, string, bool) {#add_7}

يضيف PivotTable جديدًا بتخطيط ونمط Excel 97-2003 القديم.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, int row, int column, string tableName, bool useSameSource)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceData | String | نطاق خلايا البيانات للـ PivotTable الجديد. مثال : Sheet1!A1:C8 |
| صف | Int32 | فهرس الصف للخلية في الزاوية العلوية اليسرى لنطاق الوجهة لتقرير PivotTable. |
| عمود | Int32 | فهرس العمود للخلية في الزاوية العلوية اليسرى لنطاق الوجهة لتقرير PivotTable. |
| tableName | String | اسم تقرير PivotTable الجديد. |
| useSameSource | منطقي | يشير إلى ما إذا كان يتم استخدام نفس مصدر البيانات عندما يكون جدول محوري آخر موجود قد استخدم هذا المصدر. إذا كانت الخاصية true، فستوفر الذاكرة. |

### قيمة الإرجاع

فهرس المخزن المضاف حديثًا.

### ملاحظات

ملاحظة: هذه الطريقة قديمة. إنها تعادل استدعاء PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) مع `NewPivotTableOptions.IsXlsClassic = true`. يرجى استخدام نسخة PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا من سبتمبر 2026. نعتذر عن أي إزعاج.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringInt32Int32StringBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Region");
            cells["C1"].PutValue("Sales");
            
            cells["A2"].PutValue("Product1");
            cells["B2"].PutValue("North");
            cells["C2"].PutValue(1000);
            
            cells["A3"].PutValue("Product2");
            cells["B3"].PutValue("South");
            cells["C3"].PutValue(2000);
            
            cells["A4"].PutValue("Product3");
            cells["B4"].PutValue("East");
            cells["C4"].PutValue(3000);
            
            // تحديد نطاق البيانات
            string sourceData = "A1:C4";
            
            try
            {
                // استدعاء طريقة Add مع المعلمات: (String sourceData, Int32 row, Int32 column, String tableName, Boolean useSameSource)
                int index = worksheet.PivotTables.Add(sourceData, 6, 0, "PivotTable1", false);
                
                Console.WriteLine("Pivot table added successfully at index: " + index);
                
                // الوصول إلى PivotTable الذي تم إنشاؤه حديثًا
                PivotTable pivotTable = worksheet.PivotTables[index];
                
                // تكوين جدول محوري
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product as row
                pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Region as column
                pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales as data
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, string, bool, bool) {#add_8}

يضيف PivotTable جديدًا بتخطيط ونمط Excel 97-2003 القديم.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, int row, int column, string tableName, bool useSameSource, 
    bool isXlsClassic)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceData | String | نطاق خلايا البيانات للـ PivotTable الجديد. مثال : Sheet1!A1:C8 |
| صف | Int32 | فهرس الصف للخلية في الزاوية العلوية اليسرى لنطاق الوجهة لتقرير PivotTable. |
| عمود | Int32 | فهرس العمود للخلية في الزاوية العلوية اليسرى لنطاق الوجهة لتقرير PivotTable. |
| tableName | String | اسم تقرير PivotTable الجديد. |
| useSameSource | منطقي | يشير إلى ما إذا كان يتم استخدام نفس مصدر البيانات عندما يكون جدول محوري آخر موجود قد استخدم هذا المصدر. إذا كانت الخاصية true، فستوفر الذاكرة. |
| isXlsClassic | منطقي | يشير إلى ما إذا كان يتم إضافة PivotTable كلاسيكي من Excel 97-2003. |

### قيمة الإرجاع

فهرس المخزن المضاف حديثًا.

### ملاحظات

ملاحظة: هذه الطريقة قديمة. إنها تعادل استدعاء PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) مع `NewPivotTableOptions.IsXlsClassic = true`. يرجى استخدام نسخة PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا من أكتوبر 2026. نعتذر عن أي إزعاج.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringInt32Int32StringBooleanBDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Region");
            cells["C1"].PutValue("Sales");
            cells["A2"].PutValue("Product1");
            cells["B2"].PutValue("North");
            cells["C2"].PutValue(1000);
            cells["A3"].PutValue("Product2");
            cells["B3"].PutValue("South");
            cells["C3"].PutValue(2000);
            cells["A4"].PutValue("Product3");
            cells["B4"].PutValue("East");
            cells["C4"].PutValue(3000);
            cells["A5"].PutValue("Product4");
            cells["B5"].PutValue("West");
            cells["C5"].PutValue(4000);

            // تحديد نطاق البيانات المصدر
            string sourceData = "A1:C5";

            try
            {
                // استدعِ طريقة Add مع المعلمات (String, Int32, Int32, String, Boolean, Boolean)
                int index = worksheet.PivotTables.Add(
                    sourceData,    // String sourceData
                    3,            // Int32 row - pivot table will start at row 3
                    0,            // Int32 column - pivot table will start at column 0
                    "PivotTable1", // String tableName
                    false,        // Boolean useSameSource
                    false         // Boolean isXlsClassic
                );

                Console.WriteLine("Pivot table added successfully at index: " + index);

                // تكوين جدول المحور
                PivotTable pivotTable = worksheet.PivotTables[index];
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
                pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string, bool, bool) {#add_11}

يضيف PivotTable جديدًا.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, string cell, string tableName, bool useSameSource, 
    bool isXlsClassic)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceData | String | نطاق خلايا البيانات للـ PivotTable الجديد. مثال : Sheet1!A1:C8 |
| خلية | String | الخلية في الزاوية العلوية اليسرى لنطاق الوجهة لتقرير PivotTable. |
| tableName | String | اسم تقرير PivotTable الجديد. |
| useSameSource | منطقي | يشير إلى ما إذا كان يتم استخدام نفس مصدر البيانات عندما يكون جدول محوري موجود آخر قد استخدم هذا المصدر. إذا كانت الخاصية true، فستوفر الذاكرة عندما يتم تجميع نفس مصدر البيانات في ذاكرة تخزين مؤقت محورية واحدة. |
| isXlsClassic | منطقي | يشير إلى ما إذا كان يتم إضافة PivotTable كلاسيكي من Excel 97-2003. |

### قيمة الإرجاع

فهرس المخزن المضاف حديثًا.

### ملاحظات

ملاحظة: هذه الطريقة قديمة. إنها تعادل استدعاء PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) مع `NewPivotTableOptions.IsXlsClassic = true`. يرجى استخدام نسخة PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا من أكتوبر 2026. نعتذر عن أي إزعاج.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodAddWithStringStringStringBooleanBooleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // ملء بيانات عينة
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Category");
            cells["B1"].PutValue("Product");
            cells["C1"].PutValue("Sales");
            
            for (int i = 2; i <= 10; i++)
            {
                cells["A" + i].PutValue("Cat" + (i % 3 + 1));
                cells["B" + i].PutValue("Prod" + i);
                cells["C" + i].PutValue(i * 100);
            }

            // أضف جدولًا محوريًا بالمعلمات المحددة
            int pivotTableIndex = worksheet.PivotTables.Add("=A1:C10", "E1", "SalesPivot", false, false);
            Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

            // تكوين جدول محوري
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, 0); // Category as row
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, 2); // Sum of Sales
            
            workbook.Save("PivotTableDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, string) {#add_5}

يضيف PivotTable جديد يعتمد على PivotTable آخر.

```csharp
public int Add(PivotTable pivotTable, string destCellName, string tableName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| pivotTable | PivotTable | جدول المحوري المصدر. |
| destCellName | String | الخلية في الزاوية العلوية اليسرى لنطاق الوجهة لتقرير PivotTable. |
| tableName | String | اسم تقرير PivotTable الجديد. |

### قيمة الإرجاع

فهرس PivotTable المضاف حديثًا.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithPivotTableStringStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة للجدول المحوري
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;

            // إنشاء جدول محوري من نطاق البيانات
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable sourcePivotTable = pivotTables[pivotIndex];

            try
            {
                // استدعِ طريقة Add مع المعلمات (PivotTable, String, String)
                int newPivotIndex = pivotTables.Add(sourcePivotTable, "E10", "PivotTable2");
                Console.WriteLine($"New pivot table added at index: {newPivotIndex}");

                // احفظ المصنف لإظهار التأثير
                workbook.Save("PivotTableCollectionMethodAddWithPivotTableStringStringDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, string) {#add_4}

يضيف PivotTable جديد يعتمد على PivotTable آخر.

```csharp
public int Add(PivotTable pivotTable, int row, int column, string tableName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| pivotTable | PivotTable | جدول المحوري المصدر. |
| صف | Int32 | فهرس الصف للخلية في الزاوية العلوية اليسرى لنطاق الوجهة لتقرير PivotTable. |
| عمود | Int32 | فهرس العمود للخلية في الزاوية العلوية اليسرى لنطاق الوجهة لتقرير PivotTable. |
| tableName | String | اسم تقرير PivotTable الجديد. |

### قيمة الإرجاع

فهرس PivotTable المضاف حديثًا.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithPivotTableInt32Int32StringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة للجدول المحوري
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;

            // إنشاء جدول محوري مصدر
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "C3", "SourcePivotTable");
            PivotTable sourcePivotTable = pivotTables[pivotIndex];
            sourcePivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            sourcePivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            try
            {
                // استدعِ طريقة Add مع المعلمات (PivotTable, Int32, Int32, String)
                int newPivotIndex = pivotTables.Add(sourcePivotTable, 10, 5, "NewPivotTable");
                Console.WriteLine($"New pivot table added at index: {newPivotIndex}");

                // احفظ المصنف لإظهار التأثير
                workbook.Save("PivotTableCollectionMethodAddWithPivotTableInt32Int32StringDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string[], bool, PivotPageFields, string, string) {#add_13}

يضيف كائن PivotTable جديد إلى المجموعة مع نطاقات دمج متعددة كمصدر للبيانات.

```csharp
public int Add(string[] sourceData, bool isAutoPage, PivotPageFields pageFields, 
    string destCellName, string tableName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceData | String[] | نطاقات التجميع المتعددة، مثل {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| isAutoPage | منطقي | ما إذا كان يتم إنشاء حقل صفحة واحد تلقائيًا. إذا كان true، سيتم تجاهل المعامل التالي pageFields. |
| pageFields | PivotPageFields | عناصر حقول صفحة المحور. |
| destCellName | String | destCellName اسم تقرير PivotTable الجديد. |
| tableName | String | اسم تقرير PivotTable الجديد. |

### قيمة الإرجاع

فهرس PivotTable المضاف حديثًا.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringBooleanPivotPageFieldsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            cells["A2"].Value = "Product1";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            cells["A3"].Value = "Product2";
            cells["B3"].Value = "South";
            cells["C3"].Value = 2000;
            cells["A4"].Value = "Product3";
            cells["B4"].Value = "East";
            cells["C4"].Value = 3000;

            // تحديد نطاق البيانات
            string[] sourceData = { "A1:C4" };
            bool isAutoPage = true;
            PivotPageFields pageFields = new PivotPageFields();
            string destCellName = "E5";
            string tableName = "PivotTable1";

            try
            {
                // استدعِ طريقة Add مع المعلمات المحددة
                int index = worksheet.PivotTables.Add(sourceData, isAutoPage, pageFields, destCellName, tableName);
                
                Console.WriteLine($"Pivot table added successfully at index: {index}");
                
                // الوصول إلى PivotTable الذي تم إنشاؤه حديثًا
                PivotTable pivotTable = worksheet.PivotTables[index];
                
                // تكوين حقول الجدول المحوري
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
                pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // احفظ المصنف
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotPageFields](../../pivotpagefields/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string[], bool, PivotPageFields, int, int, string) {#add_12}

يضيف كائن PivotTable جديد إلى المجموعة مع نطاقات دمج متعددة كمصدر للبيانات.

```csharp
public int Add(string[] sourceData, bool isAutoPage, PivotPageFields pageFields, int row, 
    int column, string tableName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceData | String[] | نطاقات التجميع المتعددة، مثل {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| isAutoPage | منطقي | ما إذا كان يتم إنشاء حقل صفحة واحد تلقائيًا. إذا كان true، سيتم تجاهل المعامل التالي pageFields |
| pageFields | PivotPageFields | عناصر حقول صفحة المحور. |
| صف | Int32 | فهرس الصف للخلية في الزاوية العلوية اليسرى لنطاق الوجهة لتقرير PivotTable. |
| عمود | Int32 | فهرس العمود للخلية في الزاوية العلوية اليسرى لنطاق الوجهة لتقرير PivotTable. |
| tableName | String | اسم تقرير PivotTable الجديد. |

### قيمة الإرجاع

فهرس PivotTable المضاف حديثًا.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringBooleanPivotPageFieldsDemo1
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Product1";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            
            cells["A3"].Value = "Product2";
            cells["B3"].Value = "South";
            cells["C3"].Value = 2000;
            
            cells["A4"].Value = "Product3";
            cells["B4"].Value = "East";
            cells["C4"].Value = 3000;
            
            cells["A5"].Value = "Product1";
            cells["B5"].Value = "West";
            cells["C5"].Value = 4000;
            
            cells["A6"].Value = "Product2";
            cells["B6"].Value = "North";
            cells["C6"].Value = 5000;

            // تحديد معلمات طريقة Add
            string[] sourceData = { "A1:C6" };
            bool isAutoPage = true;
            PivotPageFields pageFields = new PivotPageFields();
            int row = 8;
            int column = 1;
            string tableName = "PivotTable1";

            try
            {
                // استدعِ طريقة Add مع المعلمات المحددة
                int index = worksheet.PivotTables.Add(sourceData, isAutoPage, pageFields, row, column, tableName);
                
                Console.WriteLine($"Pivot table added successfully at index: {index}");
                
                // تكوين جدول المحور
                PivotTable pivotTable = worksheet.PivotTables[index];
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
                pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
                
                // تحديث البيانات
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotPageFields](../../pivotpagefields/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


