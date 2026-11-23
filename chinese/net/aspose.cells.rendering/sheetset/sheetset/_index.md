---
title: "SheetSet.SheetSet"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SheetSet 构造函数。根据精确的工作表索引创建工作表集合"
type: docs
url: /zh/net/aspose.cells.rendering/sheetset/sheetset/
---
## SheetSet(params int[]) {#constructor}

基于精确的工作表索引创建工作表集。

```csharp
public SheetSet(params int[] sheetIndexes)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheetIndexes | Int32[] | 基于零的工作表索引。 |

### 备注

如果遇到工作簿中不存在的工作表，渲染期间将抛出异常。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetSetMethodCtorWithInt32ArrayDemo
    {
        public static void Run()
        {
            // 创建一个包含 3 个工作表的新工作簿
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // 向每个工作表添加标识文本
            workbook.Worksheets[0].Cells["A1"].PutValue("This is Sheet 1");
            workbook.Worksheets[1].Cells["A1"].PutValue("This is Sheet 2");
            workbook.Worksheets[2].Cells["A1"].PutValue("This is Sheet 3");

            try
            {
                // 使用特定工作表索引（0 和 2）创建 SheetSet
                SheetSet sheetSet = new SheetSet(new int[] { 0, 2 });

                // 使用我们的工作表集合创建 PDF 保存选项
                PdfSaveOptions options = new PdfSaveOptions();
                options.SheetSet = sheetSet;

                // 使用选定的工作表保存工作簿
                workbook.Save("SheetSetDemo.pdf", options);
                Console.WriteLine("Created PDF containing Sheet 1 and Sheet 3");
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Invalid sheet index specified: {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## SheetSet(params string[]) {#constructor_1}

基于精确的工作表名称创建工作表集。

```csharp
public SheetSet(params string[] sheetNames)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheetNames | String[] | 工作表名称。 |

### 备注

如果遇到工作簿中不存在的工作表，渲染期间将抛出异常。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetSetMethodCtorWithStringArrayDemo
    {
        public static void Run()
        {
            // 创建一个新工作簿并添加工作表
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Name = "First";
            workbook.Worksheets.Add("Second");
            workbook.Worksheets.Add("Third");

            workbook.Worksheets["First"].Cells["A1"].PutValue("This is Sheet 1");
            workbook.Worksheets["Second"].Cells["A1"].PutValue("This is Sheet 2");
            workbook.Worksheets["Third"].Cells["A1"].PutValue("This is Sheet 3");

            // 为 SheetSet 准备工作表名称
            string[] selectedSheets = { "First", "Third" };

            try
            {
                // 使用字符串数组参数创建 SheetSet
                SheetSet sheetSet = new SheetSet(selectedSheets);

                // 使用已创建的 SheetSet 配置 PDF 保存选项
                PdfSaveOptions pdfOptions = new PdfSaveOptions();
                pdfOptions.SheetSet = sheetSet;

                // 将工作簿保存为 PDF，并使用指定的工作表
                workbook.Save("SheetSetOutput.pdf", pdfOptions);

                Console.WriteLine("Created PDF with sheets: " + string.Join(", ", selectedSheets));
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating SheetSet: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


