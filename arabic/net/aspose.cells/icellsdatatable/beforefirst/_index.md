---
title: "ICellsDataTable.BeforeFirst"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ICellsDataTable. تحريك المؤشر إلى مقدمة هذا الكائن قبل الصف الأول مباشرةً"
type: docs
url: /ar/net/aspose.cells/icellsdatatable/beforefirst/
---
## ICellsDataTable.BeforeFirst method

حرك المؤشر إلى مقدمة هذا الكائن، مباشرةً قبل الصف الأول.

```csharp
public void BeforeFirst()
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class ICellsDataTableMethodBeforeFirstDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء بيانات نموذجية
            DataTable sourceTable = new DataTable("Employees");
            sourceTable.Columns.Add("Name", typeof(string));
            sourceTable.Columns.Add("Department", typeof(string));
            sourceTable.Rows.Add("John Doe", "Engineering");
            sourceTable.Rows.Add("Jane Smith", "Marketing");

            // استيراد البيانات إلى ورقة العمل
            ImportTableOptions importOptions = new ImportTableOptions();
            importOptions.IsFieldNameShown = true;
            worksheet.Cells.ImportData(sourceTable, 0, 0, importOptions);

            // الحصول على ICellsDataTable عن طريق تصدير البيانات من ورقة العمل
            ICellsDataTable dataTable = (ICellsDataTable)worksheet.Cells.ExportDataTable(0, 0, sourceTable.Rows.Count + 1, sourceTable.Columns.Count);

            try
            {
                // إعادة تعيين المؤشر إلى بداية جدول البيانات
                dataTable.BeforeFirst();

                Console.WriteLine("Reading data from ICellsDataTable:");
                while (dataTable.Next())
                {
                    Console.WriteLine(
                        $"Name: {dataTable[0]}, " +
                        $"Department: {dataTable[1]}");
                }

                // عرض إعادة تعيين المؤشر
                dataTable.BeforeFirst();
                Console.WriteLine("\nCursor reset. Reading data again:");
                while (dataTable.Next())
                {
                    Console.WriteLine(
                        $"Name: {dataTable["Name"]}, " +
                        $"Department: {dataTable["Department"]}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing BeforeFirst method: {ex.Message}");
            }

            workbook.Save("ICellsDataTableBeforeFirstDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* interface [ICellsDataTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


