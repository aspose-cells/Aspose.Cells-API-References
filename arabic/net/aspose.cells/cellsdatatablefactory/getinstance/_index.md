---
title: "CellsDataTableFactory.GetInstance"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CellsDataTableFactory. تُنشئ ICellsDataTable من تسلسل القيم الصحيحة المعطى"
type: docs
url: /ar/net/aspose.cells/cellsdatatablefactory/getinstance/
---
## GetInstance(int[], string[]) {#getinstance_5}

ينشئ ICellsDataTable من تسلسل القيم الصحيحة المُعطى.

```csharp
public ICellsDataTable GetInstance(int[] vals, string[] columnNames)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| vals | Int32[] | قيم صحيحة لإنشاء الجدول |
| columnNames | String[] | أسماء الأعمدة للجدول. يمكن أن يكون طولها إما 1 (إنشاء الجدول بالقيم int عمودياً) أو طول القيم int (إنشاء الجدول بالقيم int أفقياً) |

### قيمة الإرجاع

مثيل ICellsDataTable

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithInt32StringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تحضير البيانات لمعلمات الطريقة (Int32[], String[])
            int[] values = new int[] { 100, 200, 300, 400, 500 };
            string[] columnNames = new string[] { "Column1", "Column2", "Column3", "Column4", "Column5" };

            try
            {
                // إنشاء مثيل CellsDataTableFactory باستخدام الانعكاس
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // استدعاء GetInstance مع معلمات (Int32[], String[])
                ICellsDataTable dataTable = factory.GetInstance(values, columnNames);

                // إخراج البيانات إلى ورقة العمل
                worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

                // عرض بعض المعلومات حول الجدول المُنشأ
                Console.WriteLine("Method executed successfully with parameters (Int32[], String[])");
                Console.WriteLine($"Created table with {dataTable.Count} rows and {dataTable.Columns.Length} columns");
                
                // طباعة أسماء الأعمدة
                Console.WriteLine("Column Names:");
                foreach (string colName in dataTable.Columns)
                {
                    Console.WriteLine(colName);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("CellsDataTableFactoryGetInstanceWithInt32StringDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(int[], bool) {#getinstance_4}

ينشئ ICellsDataTable من تسلسل القيم الصحيحة المُعطى.

```csharp
public ICellsDataTable GetInstance(int[] vals, bool vertial)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| vals | Int32[] | قيم صحيحة لإنشاء الجدول |
| عمودي | منطقي | ما إذا كان بناء الجدول بالقيم int عمودياً (true) أو أفقياً (false) |

### قيمة الإرجاع

مثيل ICellsDataTable

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithInt32ArrayBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تحضير البيانات لمعلمات الطريقة (Int32[], Boolean)
            int[] values = new int[] { 10, 20, 30, 40, 50 };
            bool vertical = true;

            try
            {
                // إنشاء مثيل CellsDataTableFactory
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // استدعاء GetInstance مع معلمات (Int32[], Boolean)
                ICellsDataTable dataTable = factory.GetInstance(values, vertical);

                // إخراج البيانات إلى ورقة العمل
                int row = 0;
                dataTable.BeforeFirst();
                while (dataTable.Next())
                {
                    for (int col = 0; col < dataTable.Columns.Length; col++)
                    {
                        worksheet.Cells[row, col].PutValue(dataTable[col]);
                    }
                    row++;
                }

                Console.WriteLine("Data table created successfully from Int32[] with vertical orientation");
                Console.WriteLine($"Total rows processed: {row}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("CellsDataTableFactoryGetInstanceWithInt32ArrayBooleanDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(double[], string[]) {#getinstance_2}

ينشئ ICellsDataTable من تسلسل القيم المزدوجة المُعطى.

```csharp
public ICellsDataTable GetInstance(double[] vals, string[] columnNames)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| vals | Double[] | قيم مزدوجة لإنشاء الجدول |
| columnNames | String[] | أسماء أعمدة الجدول. لا يمكن أن يكون طولها إلا إما 1(إنشاء جدول باستخدام القيم المزدوجة عموديًا) أو طول القيم المزدوجة(إنشاء جدول باستخدام القيم المزدوجة أفقيًا) |

### قيمة الإرجاع

مثيل ICellsDataTable

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithDoubleStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تحضير البيانات لمعلمات الطريقة (Double[], String[])
            double[] values = new double[] { 10.5, 20.25, 30.75, 40.1, 50.9 };
            string[] columnNames = new string[] { "Price", "Cost", "Margin", "Tax", "Total" };

            try
            {
                // إنشاء مثيل CellsDataTableFactory
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // استدعاء GetInstance مع معلمات (Double[], String[])
                ICellsDataTable dataTable = factory.GetInstance(values, columnNames);

                // إخراج البيانات إلى ورقة العمل
                worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

                // عرض المعلومات حول الجدول المُنشأ
                Console.WriteLine("Method executed successfully with parameters (Double[], String[])");
                Console.WriteLine($"Created table with {dataTable.Count} rows and {dataTable.Columns.Length} columns");
                
                // طباعة أسماء الأعمدة والقيم
                Console.WriteLine("Column Names:");
                foreach (string colName in dataTable.Columns)
                {
                    Console.WriteLine(colName);
                }

                // طباعة القيم
                dataTable.BeforeFirst();
                while (dataTable.Next())
                {
                    for (int i = 0; i < dataTable.Columns.Length; i++)
                    {
                        Console.WriteLine($"{dataTable.Columns[i]}: {dataTable[i]}");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("CellsDataTableFactoryGetInstanceWithDoubleStringDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(double[], bool) {#getinstance_1}

ينشئ ICellsDataTable من تسلسل القيم المزدوجة المُعطى.

```csharp
public ICellsDataTable GetInstance(double[] vals, bool vertial)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| vals | Double[] | قيم مزدوجة لإنشاء الجدول |
| عمودي | منطقي | ما إذا كان بناء الجدول باستخدام القيم المزدوجة عموديًا(true) أو أفقيًا(false) |

### قيمة الإرجاع

مثيل ICellsDataTable

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithDoubleBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تحضير البيانات لمعلمات الطريقة (Double[], Boolean)
            double[] values = new double[] { 10.5, 20.25, 30.75, 40.1, 50.9 };
            bool vertical = true;

            try
            {
                // إنشاء مثيل CellsDataTableFactory
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // استدعاء GetInstance مع (Double[], Boolean)
                ICellsDataTable dataTable = factory.GetInstance(values, vertical);

                // إخراج البيانات إلى ورقة العمل
                int row = 0;
                dataTable.BeforeFirst();
                while (dataTable.Next())
                {
                    for (int col = 0; col < dataTable.Columns.Length; col++)
                    {
                        worksheet.Cells[row, col].PutValue(dataTable[col]);
                    }
                    row++;
                }

                Console.WriteLine("Data table created successfully with parameters (Double[], Boolean)");
                Console.WriteLine($"Total rows processed: {row}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("CellsDataTableFactoryGetInstanceWithDoubleBooleanDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(object[], string[]) {#getinstance_10}

ينشئ ICellsDataTable من تسلسل الكائنات المُعطى.

```csharp
public ICellsDataTable GetInstance(object[] vals, string[] columnNames)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| vals | Object[] | الكائنات لبناء الجدول |
| columnNames | String[] | أسماء أعمدة الجدول. لا يمكن أن يكون طولها إلا إما 1(إنشاء جدول باستخدام الكائنات عموديًا) أو طول الكائنات(إنشاء جدول باستخدام الكائنات أفقيًا) |

### قيمة الإرجاع

مثيل ICellsDataTable

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithObjectStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تحضير البيانات لمعلمات الطريقة (Object[], String[])
            object[] values = new object[] { "John Doe", 35, 75000.50, DateTime.Now };
            string[] columnNames = new string[] { "Name", "Age", "Salary", "Hire Date" };

            try
            {
                // إنشاء مثيل CellsDataTableFactory باستخدام الانعكاس
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // استدعاء طريقة GetInstance مع معلمات (Object[], String[])
                ICellsDataTable dataTable = factory.GetInstance(values, columnNames);

                // إخراج البيانات إلى ورقة العمل باستخدام ImportData بدلاً من ImportDataTable
                worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

                Console.WriteLine("Method executed successfully with parameters (Object[], String[])");
                Console.WriteLine($"Created table with {dataTable.Count} rows and {dataTable.Columns.Length} columns");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("CellsDataTableFactoryGetInstanceWithObjectStringDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(object[][], bool, string[]) {#getinstance_11}

ينشئ ICellsDataTable من تسلسل الكائنات المُعطى.

```csharp
public ICellsDataTable GetInstance(object[][] vals, bool hasHeader, string[] columnNames)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| vals | Object[][] | الكائنات لبناء الجدول |
| hasHeader | منطقي | يشير إلى ما إذا كان الصف الأول هو صف رأس. |
| columnNames | String[] | أسماء أعمدة الجدول. لا يمكن أن يكون طولها إلا إما 1(إنشاء جدول باستخدام الكائنات عموديًا) أو طول الكائنات(إنشاء جدول باستخدام الكائنات أفقيًا) |

### قيمة الإرجاع

مثيل ICellsDataTable

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithObjectBooleanStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تحضير البيانات لمعلمات الطريقة (Object[][], Boolean, String[])
            object[][] data = new object[][]
            {
                new object[] { "ID", "Name", "Price" },
                new object[] { 1, "Laptop", 999.99 },
                new object[] { 2, "Phone", 699.99 },
                new object[] { 3, "Tablet", 399.99 }
            };

            bool hasHeader = true;
            string[] columnNames = new string[] { "ProductID", "ProductName", "ProductPrice" };

            try
            {
                // إنشاء مثيل CellsDataTableFactory
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // استدعاء GetInstance مع (Object[][], Boolean, String[])
                ICellsDataTable dataTable = factory.GetInstance(data, hasHeader, columnNames);

                // إخراج البيانات إلى ورقة العمل
                int row = 0;
                dataTable.BeforeFirst();
                while (dataTable.Next())
                {
                    for (int col = 0; col < dataTable.Columns.Length; col++)
                    {
                        worksheet.Cells[row, col].PutValue(dataTable[col]);
                    }
                    row++;
                }

                Console.WriteLine("Data table created successfully with parameters (Object[][], Boolean, String[])");
                Console.WriteLine($"Total rows processed: {row}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("CellsDataTableFactoryGetInstanceWithObjectBooleanStringDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(object[], bool) {#getinstance_9}

ينشئ ICellsDataTable من تسلسل الكائنات المُعطى.

```csharp
public ICellsDataTable GetInstance(object[] vals, bool vertial)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| vals | Object[] | الكائنات لبناء الجدول |
| عمودي | منطقي | ما إذا كان بناء الجدول باستخدام الكائنات عموديًا(true) أو أفقيًا(false) |

### قيمة الإرجاع

مثيل ICellsDataTable

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithObjectBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تحضير البيانات لمعلمات الطريقة (Object[], Boolean)
            object[] data = new object[] { "Product", "Price", "Stock", "Available" };
            bool vertical = true;

            try
            {
                // إنشاء مثيل CellsDataTableFactory باستخدام الانعكاس
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // استدعاء GetInstance مع معلمات (Object[], Boolean)
                ICellsDataTable dataTable = factory.GetInstance(data, vertical);

                // إخراج البيانات إلى ورقة العمل
                dataTable.BeforeFirst();
                int row = 0;
                while (dataTable.Next())
                {
                    for (int col = 0; col < dataTable.Columns.Length; col++)
                    {
                        worksheet.Cells[row, col].PutValue(dataTable[col]);
                    }
                    row++;
                }

                Console.WriteLine("Data table created successfully with parameters (Object[], Boolean)");
                Console.WriteLine($"Data orientation: {(vertical ? "Vertical" : "Horizontal")}");
                Console.WriteLine($"Total items processed: {dataTable.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("CellsDataTableFactoryGetInstanceWithObjectBooleanDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(int[]) {#getinstance_3}

```csharp
public ICellsDataTable GetInstance(int[] vals)
```

### انظر أيضًا

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(double[]) {#getinstance}

```csharp
public ICellsDataTable GetInstance(double[] vals)
```

### انظر أيضًا

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(object[]) {#getinstance_8}

```csharp
public ICellsDataTable GetInstance(object[] vals)
```

### انظر أيضًا

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(ICollection) {#getinstance_6}

ينشئ ICellsDataTable من مجموعة مُعطاة.

```csharp
public ICellsDataTable GetInstance(ICollection collection)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| مجموعة | ICollection | المجموعة لبناء الجدول |

### قيمة الإرجاع

مثيل ICellsDataTable

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellsDataTableFactoryMethodGetInstanceWithICollectionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تحضير ArrayList كـ ICollection
            ArrayList data = new ArrayList
            {
                new ArrayList { "Product", "Price", "Stock" },
                new ArrayList { "Keyboard", 49.99, 120 },
                new ArrayList { "Mouse", 29.99, 200 },
                new ArrayList { "Monitor", 199.99, 35 }
            };

            try
            {
                // إنشاء مثيل CellsDataTableFactory
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // استدعاء GetInstance مع معلمة ICollection
                ICellsDataTable dataTable = factory.GetInstance(data);

                // إخراج البيانات إلى ورقة العمل
                int row = 0;
                dataTable.BeforeFirst();
                while (dataTable.Next())
                {
                    for (int col = 0; col < dataTable.Columns.Length; col++)
                    {
                        worksheet.Cells[row, col].PutValue(dataTable[col]);
                    }
                    row++;
                }

                Console.WriteLine("Data table created successfully from ICollection");
                Console.WriteLine($"Total rows processed: {row}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("CellsDataTableFactoryGetInstanceWithICollectionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(ICollection, bool) {#getinstance_7}

ينشئ ICellsDataTable من مجموعة مُعطاة.

```csharp
public ICellsDataTable GetInstance(ICollection collection, bool hasHeader)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| مجموعة | ICollection | المجموعة لبناء الجدول |
| hasHeader | منطقي | يشير إلى ما إذا كان الصف الأول هو رأس |

### قيمة الإرجاع

مثيل ICellsDataTable

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellsDataTableFactoryMethodGetInstanceWithICollectionBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تحضير جمع البيانات لمعلمات الطريقة (ICollection, Boolean)
            ArrayList dataCollection = new ArrayList
            {
                new { Product = "Apple", Price = 2.5, Stock = 100 },
                new { Product = "Orange", Price = 1.8, Stock = 150 },
                new { Product = "Banana", Price = 0.9, Stock = 200 }
            };
            bool hasHeader = true;

            try
            {
                // إنشاء مثيل CellsDataTableFactory
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // استدعاء GetInstance مع معلمات (ICollection, Boolean)
                ICellsDataTable dataTable = factory.GetInstance(dataCollection, hasHeader);

                // إخراج البيانات إلى ورقة العمل
                worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

                // عرض المعلومات حول الجدول المُنشأ
                Console.WriteLine("Method executed successfully with parameters (ICollection, Boolean)");
                Console.WriteLine($"Created table with {dataTable.Count} rows and {dataTable.Columns.Length} columns");
                
                // طباعة أسماء الأعمدة
                Console.WriteLine("Column Names:");
                foreach (string colName in dataTable.Columns)
                {
                    Console.WriteLine(colName);
                }

                // طباعة القيم
                dataTable.BeforeFirst();
                while (dataTable.Next())
                {
                    for (int i = 0; i < dataTable.Columns.Length; i++)
                    {
                        Console.WriteLine($"{dataTable.Columns[i]}: {dataTable[i]}");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("CellsDataTableFactoryGetInstanceWithICollectionBooleanDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


