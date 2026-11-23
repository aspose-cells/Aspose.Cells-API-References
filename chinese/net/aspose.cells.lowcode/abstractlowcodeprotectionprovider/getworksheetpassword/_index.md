---
title: "AbstractLowCodeProtectionProvider.GetWorksheetPassword"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "AbstractLowCodeProtectionProvider 方法。获取用于保护指定工作表的密码"
type: docs
url: /zh/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworksheetpassword/
---
## AbstractLowCodeProtectionProvider.GetWorksheetPassword method

获取保护指定工作表的密码。

```csharp
public virtual string GetWorksheetPassword(string sheetName)
```

### 返回值

用于保护指定工作表的密码。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetWorksheetPasswordWithStringDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿并访问第一个工作表
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            string sheetName = worksheet.Name;

            // 创建自定义保护提供程序实例
            var provider = new CustomProtectionProvider();

            try
            {
                // 使用工作表名称调用 GetWorksheetPassword
                string password = provider.GetWorksheetPassword(sheetName);

                // 使用检索到的密码对工作表应用保护
                worksheet.Protect(ProtectionType.All, password, null);

                Console.WriteLine($"Protected worksheet '{sheetName}' with password: {password}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetWorksheetPassword: {ex.Message}");
            }

            // 保存受保护的工作簿
            workbook.Save("WorksheetPasswordDemo.xlsx");

        }
    }

    // 基于工作表名称返回密码的自定义实现
    public class CustomProtectionProvider : AbstractLowCodeProtectionProvider
    {
        public new string GetWorksheetPassword(string sheetName)
        {
            // 用于演示的简单密码生成逻辑
            return $"pw_{sheetName}";
        }
    }
}
```

### 另请参见

* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


