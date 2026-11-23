---
title: "HtmlSaveOptions.ExportObjectListener"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "HtmlSaveOptions 属性。获取或设置用于导出对象的 ExportObjectListener"
type: docs
url: /zh/net/aspose.cells/htmlsaveoptions/exportobjectlistener/
---
## HtmlSaveOptions.ExportObjectListener property

获取或设置用于导出对象的 ExportObjectListener。

```csharp
[Obsolete("Use HtmlSaveOptions.IStreamProvider property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IExportObjectListener ExportObjectListener { get; set; }
```

### 备注

注意：此属性已过时。请改用 HtmlSaveOptions.IStreamProvider 属性。该属性将在自 2015 年 8 月起的 12 个月后移除。Aspose 对您可能遇到的任何不便表示歉意。

### 示例

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportObjectListenerDemo
    {
        public static void Run()
        {
            // 创建自定义导出对象监听器
            var listener = new CustomExportObjectListener();
            
            // 使用示例数据创建工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Export Object Listener");
            
            // 使用监听器创建 HTML 保存选项
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                ExportObjectListener = listener
            };

            // 保存为 HTML 文件
            workbook.Save("output.html", saveOptions);
        }
    }

    // IExportObjectListener 的自定义实现
    public class CustomExportObjectListener : IExportObjectListener
    {
        public object ExportObject(ExportObjectEvent e)
        {
            // 示例：处理导出的对象
            Console.WriteLine($"Exporting object: {e.GetType()}");
            // 返回原始对象（如有需要可进行修改）
            return e;
        }
    }
}
```

### 另请参见

* interface [IExportObjectListener](../../iexportobjectlistener/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


