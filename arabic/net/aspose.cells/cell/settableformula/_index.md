---
title: "Cell.SetTableFormula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Cell method. إنشاء جدول بيانات بمتغيرين للنطاق المحدد بدءًا من هذه الخلية"
type: docs
url: /ar/net/aspose.cells/cell/settableformula/
---
## SetTableFormula(int, int, string, string, object[][]) {#settableformula_3}

إنشاء جدول بيانات بمتغيرين للنطاق المحدد بدءًا من هذه الخلية.

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, string rowInputCell, 
    string columnInputCell, object[][] values)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| rowNumber | Int32 | عدد الصفوف لتعبئة الصيغة. |
| columnNumber | Int32 | عدد الأعمدة لتعبئة الصيغة. |
| rowInputCell | String | خلية إدخال الصف |
| columnInputCell | String | خلية إدخال العمود |
| القيم | Object[][] | القيم للخلايا في نطاق صيغة الجدول |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32StringStringObjectArrayDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cells cells = workbook.Worksheets[0].Cells;
            cells[1, 1].Formula = "=A1+A2";

            cells[1, 2].PutValue(2);
            cells[1, 3].PutValue(3);
            cells[2, 1].PutValue(2);
            cells[3, 1].PutValue(3);
            cells[4, 1].PutValue(4);

            // الخلية الهدف حيث سيتم تعيين صيغة الجدول
            Cell targetCell = worksheet.Cells["C3"];

            // تحضير المعلمات لـ SetTableFormula
            int rowNumber = 3;
            int columnNumber = 2;
            string rowInputCell = "A1";
            string columnInputCell = "A2";
            object[][] values = new object[][]
            {
                new object[] { 1, 2 },    // Row 1 data
                new object[] { 3, 4 },    // Row 2 data
                new object[] { 5, 6 }     // Row 3 data
            };

            try
            {
                // تعيين صيغة الجدول على الخلية الهدف
                targetCell.SetTableFormula(rowNumber, columnNumber, rowInputCell, columnInputCell, values);

                // حساب صيغ دفتر العمل لتحديث النتائج
                workbook.CalculateFormula();

                Console.WriteLine("Table formula set successfully. Check D1:" + targetCell.StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting table formula: {ex.Message}");
            }

            // احفظ المصنف المعدل
            workbook.Save("SetTableFormulaDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetTableFormula(int, int, string, bool, object[][]) {#settableformula_2}

إنشاء جدول بيانات بمتغير واحد للنطاق المحدد بدءًا من هذه الخلية.

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, string inputCell, bool isRowInput, 
    object[][] values)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| rowNumber | Int32 | عدد الصفوف لتعبئة الصيغة. |
| columnNumber | Int32 | عدد الأعمدة لتعبئة الصيغة. |
| inputCell | String | خلية الإدخال |
| isRowInput | منطقي | يشير إلى ما إذا كانت خلية الإدخال هي خلية إدخال صف (true) أو خلية إدخال عمود (false). |
| القيم | Object[][] | القيم للخلايا في نطاق صيغة الجدول |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32StringBooleanObjectDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد والوصول إلى الورقة الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cells cells = worksheet.Cells;
            cells[1, 1].Formula = "=A1+A2";

            cells[1, 2].PutValue(100000);
            cells[1, 3].PutValue(0.05);
            cells[1, 4].PutValue(2);
            cells[2, 1].PutValue(360);
            cells[3, 1].PutValue(30);
            cells[4, 1].PutValue(40);
            
            try
            {
                // تحضير المعلمات لـ SetTableFormula
                int rowCount = 3;
                int colCount = 3;
                object[][] inputValues = new object[][] 
                {
                    new object[] { 0.05, 0.06, 0.07 },
                    new object[] { 1000, 2000, 3000 },
                    new object[] { 100, 200, 300 }
                };

                // الحصول على الخلية الهدف لجدول البيانات (C3)
                Cell tableCell = worksheet.Cells["C3"];
                // استدعاء SetTableFormula مع تغيرات معدل الفائدة
                tableCell.SetTableFormula(
                    rowNumber: rowCount,
                    columnNumber: colCount,
                    inputCell: "A1",
                    isRowInput: true,
                    values: inputValues
                );

                // حساب الصيغ لتحديث نتائج الجدول
                workbook.CalculateFormula();

                Console.WriteLine("Data table created successfully with varying interest rates");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating data table: {ex.Message}");
            }

            // احفظ المصنف المعدل
            workbook.Save("SetTableFormulaDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetTableFormula(int, int, int, int, int, int, object[][]) {#settableformula_1}

إنشاء جدول بيانات بمتغيرين للنطاق المحدد بدءًا من هذه الخلية.

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, 
    int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, 
    object[][] values)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| rowNumber | Int32 | عدد الصفوف لتعبئة الصيغة. |
| columnNumber | Int32 | عدد الأعمدة لتعبئة الصيغة. |
| rowIndexOfRowInputCell | Int32 | فهرس الصف لخلية إدخال الصف |
| columnIndexOfRowInputCell | Int32 | فهرس العمود للخلية المدخلة للصف |
| rowIndexOfColumnInputCell | Int32 | فهرس الصف للخلية المدخلة للعمود |
| columnIndexOfColumnInputCell | Int32 | فهرس العمود للخلية المدخلة للعمود |
| القيم | Object[][] | القيم للخلايا في نطاق صيغة الجدول |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells[1, 1].Formula = "=A1+A2";

            cells[1, 2].PutValue(2);
            cells[1, 3].PutValue(3);
            cells[1, 4].PutValue(4);
            cells[2, 1].PutValue(2);
            cells[3, 1].PutValue(3);
            cells[4, 1].PutValue(4);
            
            Cell formulaCell = cells[2, 2];

            // تحضير قيم الإدخال لجدول البيانات (معدلات الفائدة ومبالغ القرض)
            object[][] tableValues = new object[3][];
            tableValues[0] = new object[] { 0.05, 0.06, 0.07 };
            tableValues[1] = new object[] { 1000, 2000, 3000 };
            tableValues[2] = new object[] { 100, 200, 300 };

            try
            {
                // تعيين صيغة الجدول بأبعاد جدول بيانات 3x3 وإزاحات خلية الإدخال
                formulaCell.SetTableFormula(
                    rowNumber: 3,
                    columnNumber: 3,
                    rowIndexOfRowInputCell: 0,  
                    columnIndexOfRowInputCell: 0,   
                    rowIndexOfColumnInputCell: 1,   
                    columnIndexOfColumnInputCell: 0, 
                    values: tableValues
                );

                workbook.CalculateFormula();
                Console.WriteLine("Data table formula set successfully. Check B2:D4 in output.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting table formula: {ex.Message}");
            }

            workbook.Save("CellTableFormulaDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetTableFormula(int, int, int, int, bool, object[][]) {#settableformula}

إنشاء جدول بيانات بمتغير واحد للنطاق المحدد بدءًا من هذه الخلية.

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, 
    int columnIndexOfInputCell, bool isRowInput, object[][] values)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| rowNumber | Int32 | عدد الصفوف لتعبئة الصيغة. |
| columnNumber | Int32 | عدد الأعمدة لتعبئة الصيغة. |
| rowIndexOfInputCell | Int32 | فهرس الصف للخلية المدخلة |
| columnIndexOfInputCell | Int32 | فهرس العمود للخلية المدخلة |
| isRowInput | منطقي | يشير إلى ما إذا كانت خلية الإدخال هي خلية إدخال صف (true) أو خلية إدخال عمود (false). |
| القيم | Object[][] | القيم للخلايا في نطاق صيغة الجدول |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32Int32Int32BooleanObjDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد والوصول إلى الورقة الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cells cells = workbook.Worksheets[0].Cells;
            cells[1, 1].Formula = "=A1+A2";

            cells[1, 2].PutValue(20);
            cells[1, 3].PutValue(30);            
            cells[2, 1].PutValue(20);
            cells[3, 1].PutValue(30);
            cells[4, 1].PutValue(40);

            // إنشاء مصفوفة بيانات عينة لمعلمات صيغة الجدول
            object[][] inputValues = new object[][]
            {
                new object[] { 10, 20 },
                new object[] { 30, 40 },
                new object[] { 50, 60 }
            };

            // الحصول على الخلية المستهدفة لتطبيق صيغة الجدول
            Cell formulaCell = worksheet.Cells[2, 2];

            try
            {
                // تعيين صيغة الجدول بـ: 
                // 3 صفوف، 2 أعمدة، خلية الإدخال في A1 (0,0)، 
                // نوع إدخال الصف، والقيم العينة
                formulaCell.SetTableFormula(
                    rowNumber: 3,
                    columnNumber: 2,
                    rowIndexOfInputCell: 0,
                    columnIndexOfInputCell: 0,
                    isRowInput: true,
                    values: inputValues
                );

                workbook.CalculateFormula();
                Console.WriteLine("Table formula applied successfully. " + 
                    "Saved workbook with 3x2 table formula at C3.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting table formula: {ex.Message}");
            }

            // احفظ المصنف المعدل
            workbook.Save("TableFormulaDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


