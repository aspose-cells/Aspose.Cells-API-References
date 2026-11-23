---
title: "PclSaveOptions.PclSaveOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PclSaveOptions 构造函数。创建用于保存 pcl 文件的选项"
type: docs
url: /zh/net/aspose.cells/pclsaveoptions/pclsaveoptions/
---
## PclSaveOptions constructor

创建用于保存 pcl 文件的选项。

```csharp
public PclSaveOptions()
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PclSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 向工作表添加一些示例数据
            worksheet.Cells["A1"].PutValue("PCL Save Options Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates PclSaveOptions constructor");
            
            try
            {
                // 调用 #ctor 方法以创建 PclSaveOptions 实例
                PclSaveOptions pclOptions = new PclSaveOptions();
                
                // 如有需要，配置其他选项
                pclOptions.AddPrinterFont("Arial", "ArialPCL");
                
                Console.WriteLine("PclSaveOptions created successfully");
                
                // 使用 PCL 选项保存工作簿
                workbook.Save("PclSaveOptionsDemo.pcl", pclOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating PclSaveOptions: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [PclSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


