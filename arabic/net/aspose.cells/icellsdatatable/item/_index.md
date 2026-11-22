---
title: "ICellsDataTable.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ICellsDataTable. تحصل على البيانات المخزنة في العمود المحدد بواسطة الفهرس"
type: docs
url: /ar/net/aspose.cells/icellsdatatable/item/
---
## ICellsDataTable indexer (1 of 2)

يحصل على البيانات المخزنة في العمود المحدد بواسطة الفهرس.

```csharp
public object this[int columnIndex] { get; }
```

| معامل | الوصف |
| --- | --- |
| columnIndex | الفهرس الصفري للعمود. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ICellsDataTablePropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء ICellsDataTable مخصص مع بيانات نموذجية
            ICellsDataTable dataTable = new SampleDataTable();

            // إعادة تعيين موضع المؤشر
            dataTable.BeforeFirst();

            Console.WriteLine("Reading data using Item property:");
            while (dataTable.Next())
            {
                // الوصول إلى القيم بواسطة فهرس العمود
                Console.WriteLine($"Product: {dataTable[0]}, Price: {dataTable[1]}, Stock: {dataTable[2]}");

                // الوصول إلى القيم بواسطة اسم العمود
                Console.WriteLine($"Product: {dataTable["Product"]}, Price: {dataTable["Price"]}, Stock: {dataTable["Stock"]}\n");
            }
        }
    }

    internal class SampleDataTable : ICellsDataTable
    {
        private readonly string[] columns = { "Product", "Price", "Stock" };
        private readonly object[][] data = 
        {
            new object[] { "Laptop", 999.99, 15 },
            new object[] { "Phone", 699.99, 25 },
            new object[] { "Tablet", 299.99, 50 }
        };
        private int currentRow = -1;

        public string[] Columns => columns;
        public int Count => data.Length;

        public object this[int columnIndex] => data[currentRow][columnIndex];
        public object this[string columnName] => data[currentRow][Array.IndexOf(columns, columnName)];

        public void BeforeFirst() => currentRow = -1;
        public bool Next() => ++currentRow < data.Length;
    }
}
```

### انظر أيضًا

* interface [ICellsDataTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ICellsDataTable indexer (2 of 2)

يحصل على البيانات المخزنة في العمود المحدد باسم العمود.

```csharp
public object this[string columnName] { get; }
```

| معامل | الوصف |
| --- | --- |
| columnName | اسم العمود. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ICellsDataTablePropertyItemDemo1
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ملء البيانات النموذجية في الخلايا
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(499.99);

            // تصدير نطاق البيانات إلى ICellsDataTable باستخدام تحويل صريح
            ICellsDataTable dataTable = (ICellsDataTable)worksheet.Cells.ExportDataTable(0, 0, 3, 2);

            // الانتقال إلى ما قبل السجل الأول
            dataTable.BeforeFirst();

            Console.WriteLine("Reading data table values:");
            while (dataTable.Next())
            {
                // الوصول إلى خاصية Item باستخدام أسماء الأعمدة (المؤشر)
                string product = dataTable["Product"].ToString();
                double price = Convert.ToDouble(dataTable["Price"]);

                Console.WriteLine($"Item[Product]: {product}, Item[Price]: {price}");
            }

            // احفظ المصنف
            workbook.Save("ItemPropertyDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* interface [ICellsDataTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


