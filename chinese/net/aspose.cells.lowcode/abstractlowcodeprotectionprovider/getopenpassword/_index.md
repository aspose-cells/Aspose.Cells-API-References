---
title: "AbstractLowCodeProtectionProvider.GetOpenPassword"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "AbstractLowCodeProtectionProvider 方法。获取打开电子表格文件的密码"
type: docs
url: /zh/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getopenpassword/
---
## AbstractLowCodeProtectionProvider.GetOpenPassword method

获取打开电子表格文件的密码。

```csharp
public virtual string GetOpenPassword()
```

### 返回值

用于打开电子表格文件的密码。为空表示打开文件时没有保护。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetOpenPasswordDemo
    {
        public static void Run()
        {
            try
            {
                // 创建保护提供程序实例
                var protectionProvider = new DemoProtectionProvider();

                // 调用 GetOpenPassword 方法以检索密码
                string password = protectionProvider.GetOpenPassword();

                // 创建一个新的工作簿并应用密码
                Workbook workbook = new Workbook("sample.xlsx");
                workbook.Settings.Password = password;

                // 保存受密码保护的工作簿
                workbook.Save("MethodGetOpenPasswordDemo.xlsx");

                Console.WriteLine($"Workbook protected with open password: {password}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing demo: {ex.Message}");
            }
        }
    }

    public class DemoProtectionProvider : AbstractLowCodeProtectionProvider
    {
        public override string GetOpenPassword()
        {
            return "AsposeDemo123!";
        }
    }
}
```

### 另请参见

* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


