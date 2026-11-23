---
title: "LowCodeSaveOptions.OutputStream"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "LowCodeSaveOptions 属性。获取和设置用于写入生成数据的 Stream。当将此属性设置为非 null 值时，OutputFile 将被忽略"
type: docs
url: /zh/net/aspose.cells.lowcode/lowcodesaveoptions/outputstream/
---
## LowCodeSaveOptions.OutputStream property

获取和设置用于写入生成数据的 Stream。当将此属性设置为非 null 值时，[`OutputFile`](../outputfile/) 将被忽略。

```csharp
public Stream OutputStream { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class LowCodeSaveOptionsPropertyOutputStreamDemo
    {
        public static void Run()
        {
            // 创建包含示例数据的新工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample OutputStream Demo");

            try
            {
                // 创建 LowCodeSaveOptions 实例
                LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
                
                // 创建用于演示的内存流
                using (MemoryStream stream = new MemoryStream())
                {
                    // 设置 OutputStream 属性
                    saveOptions.OutputStream = stream;
                    saveOptions.SaveFormat = SaveFormat.Xlsx;

                    // 使用这些选项保存（将写入我们的内存流）
                    workbook.Save(saveOptions.OutputStream, saveOptions.SaveFormat);

                    // 验证流已被写入
                    Console.WriteLine($"OutputStream length: {saveOptions.OutputStream.Length} bytes");
                    Console.WriteLine("OutputStream position reset to 0 for reading");
                    saveOptions.OutputStream.Position = 0;

                    // 从流创建新工作簿以验证内容
                    Workbook verifyWorkbook = new Workbook(saveOptions.OutputStream);
                    Console.WriteLine($"Verified worksheet count: {verifyWorkbook.Worksheets.Count}");
                }
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

* class [LowCodeSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


