---
title: "PclSaveOptions.EmbedFont"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PclSaveOptions 属性。指示是否将字体嵌入输出的 Pcl 文件中"
type: docs
url: /zh/net/aspose.cells/pclsaveoptions/embedfont/
---
## PclSaveOptions.EmbedFont property

指示是否将字体嵌入输出的 Pcl 文件中。

```csharp
public bool EmbedFont { get; set; }
```

### 备注

默认值为 true。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PclSaveOptionsPropertyEmbedFontDemo
    {
        public static void Run()
        {
            // 创建新工作簿并添加一些示例数据
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Demonstrating EmbedFont property");
            sheet.Cells["A2"].PutValue(DateTime.Now);

            try
            {
                // 创建 PCL 保存选项
                PclSaveOptions pclOptions = new PclSaveOptions();

                // 读取并显示 EmbedFont 属性的当前值
                Console.WriteLine("Current EmbedFont value: " + pclOptions.EmbedFont);

                // （可选）如果属性是可写的，你可以设置它，但这里我们只读取它
                // pclOptions.EmbedFont = true;

                // 使用这些选项将工作簿保存为 PCL 文件
                workbook.Save("EmbedFontDemo.pcl", pclOptions);

                Console.WriteLine("Workbook saved successfully with EmbedFont demonstration.");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### 另请参见

* class [PclSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


