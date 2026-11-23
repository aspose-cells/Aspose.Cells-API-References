---
title: "EbookSaveOptions.EbookSaveOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "EbookSaveOptions 构造函数。创建用于保存电子书文件的选项"
type: docs
url: /zh/net/aspose.cells.saving/ebooksaveoptions/ebooksaveoptions/
---
## EbookSaveOptions() {#constructor}

创建用于保存电子书文件的选项。

```csharp
public EbookSaveOptions()
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class EbookSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // 创建包含示例数据的新工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 添加示例内容
            worksheet.Cells["A1"].PutValue("Ebook Test");
            worksheet.Cells["A2"].PutValue("This is a test for EbookSaveOptions");
            
            // 使用构造函数创建 EbookSaveOptions
            EbookSaveOptions saveOptions = new EbookSaveOptions();
            
            // 使用 EbookSaveOptions 保存工作簿（自动保存为 EPUB）
            workbook.Save("output.epub", saveOptions);
            
            Console.WriteLine("Ebook saved successfully with EbookSaveOptions constructor.");
        }
    }
}
```

### 另请参见

* class [EbookSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)

---

## EbookSaveOptions(SaveFormat) {#constructor_1}

创建用于保存电子书文件的选项。

```csharp
public EbookSaveOptions(SaveFormat saveFormat)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| saveFormat | SaveFormat | 文件格式。应为 Epub 或 Azw3。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class EbookSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 向工作表添加示例数据
            worksheet.Cells["A1"].PutValue("Sample Ebook Content");
            
            try
            {
                // 使用 SaveFormat 参数调用 #ctor 方法
                EbookSaveOptions saveOptions = new EbookSaveOptions(SaveFormat.Epub);
                
                // 如有需要，设置其他属性
                saveOptions.Encoding = System.Text.Encoding.UTF8;
                
                Console.WriteLine("EbookSaveOptions constructor executed successfully with SaveFormat.Epub");
                
                // 使用创建的选项保存工作簿
                workbook.Save("EbookSaveOptionsDemo.epub", saveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing EbookSaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [EbookSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


