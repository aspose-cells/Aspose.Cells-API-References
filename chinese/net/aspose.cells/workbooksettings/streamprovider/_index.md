---
title: "WorkbookSettings.StreamProvider"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "WorkbookSettings 属性。获取和设置外部资源的流提供程序"
type: docs
url: /zh/net/aspose.cells/workbooksettings/streamprovider/
---
## WorkbookSettings.StreamProvider property

获取和设置外部资源的流提供程序。

```csharp
[Obsolete("Use ResourceProvider property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IStreamProvider StreamProvider { get; set; }
```

### 备注

NOTE: 此成员现已过时。请改用 ResourceProvider 属性。此属性将在自 2022 年 6 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CustomStreamProvider1 : IStreamProvider
    {
        private MemoryStream stream;

        public void InitStream(StreamProviderOptions options)
        {
            stream = new MemoryStream();
            options.Stream = stream;
        }

        public void CloseStream(StreamProviderOptions options)
        {
            stream.Close();
            Console.WriteLine($"Stream closed. Content length: {stream.Length} bytes");
        }
    }

    public class WorkbookSettingsPropertyStreamProviderDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 访问工作簿设置
            WorkbookSettings settings = workbook.Settings;

            // 显示当前 StreamProvider 值
            Console.WriteLine("Current StreamProvider value: " + (settings.StreamProvider == null ? "null" : "custom provider"));

            // 设置自定义流提供程序
            settings.StreamProvider = new CustomStreamProvider1();

            // 添加一些数据以演示流的使用
            worksheet.Cells["A1"].PutValue("Test data for stream provider");

            // 保存工作簿 - 这将触发流提供程序
            workbook.Save("PropertyStreamProviderDemo.xlsx");

            // 重置流提供程序
            settings.StreamProvider = null;
            Console.WriteLine("StreamProvider reset to null");
        }
    }
}
```

### 另请参见

* interface [IStreamProvider](../../istreamprovider/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


