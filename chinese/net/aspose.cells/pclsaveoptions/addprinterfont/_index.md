---
title: "PclSaveOptions.AddPrinterFont"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PclSaveOptions 方法。添加已由制造商预装到打印机的字体信息"
type: docs
url: /zh/net/aspose.cells/pclsaveoptions/addprinterfont/
---
## PclSaveOptions.AddPrinterFont method

添加关于已由制造商添加到打印机的字体的信息。

```csharp
public void AddPrinterFont(string fontFullName, string fontPclName)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fontFullName | String | 源文件中使用的字体的完整名称（例如 "Times New Roman Bold Italic"）。 |
| fontPclName | String | 将在输出 Pcl 文档中使用的字体名称。 |

### 备注

根据 Pcl 规范，任何打印机都内置 52 种字体。不过制造商可以向其设备添加其他字体。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PclSaveOptionsMethodAddPrinterFontWithStringStringDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 向工作表添加一些文本以演示字体使用
            worksheet.Cells["A1"].PutValue("This text will use the added printer font");
            
            // 创建 PCL 保存选项
            PclSaveOptions pclSaveOptions = new PclSaveOptions();
            
            try
            {
                // 使用特定字体名称调用 AddPrinterFont 方法
                pclSaveOptions.AddPrinterFont("Arial", "ArialPCL");
                pclSaveOptions.AddPrinterFont("Times New Roman", "TimesPCL");
                
                Console.WriteLine("AddPrinterFont method executed successfully with parameters (String, String)");
                
                // 使用 PCL 选项保存工作簿
                workbook.Save("PclWithAddedPrinterFonts.pcl", pclSaveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddPrinterFont method: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [PclSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


