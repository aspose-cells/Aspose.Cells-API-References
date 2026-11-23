---
title: "AbstractLowCodeProtectionProvider.GetWritePassword"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "AbstractLowCodeProtectionProvider 方法。获取用于修改电子表格文件的密码"
type: docs
url: /zh/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getwritepassword/
---
## AbstractLowCodeProtectionProvider.GetWritePassword method

获取修改电子表格文件的密码。

```csharp
public virtual string GetWritePassword()
```

### 返回值

用于修改电子表格文件的密码。空表示对文件的修改没有保护。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetWritePasswordDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // 创建自定义保护提供程序实例
            var protectionProvider = new CustomProtectionProvider();

            try
            {
                // 显式调用 GetWritePassword 并显示结果
                string writePassword = protectionProvider.GetWritePassword();
                Console.WriteLine($"Retrieved write password: {writePassword}");

                // 保存工作簿 - 直接应用写入保护
                workbook.Settings.WriteProtection.Password = writePassword;
                workbook.Save("MethodGetWritePasswordDemo.xlsx");
                Console.WriteLine("Workbook saved with write protection password.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetWritePassword method: {ex.Message}");
            }
        }

    }

    // 自定义保护提供程序实现
    public class CustomProtectionProvider : AbstractLowCodeProtectionProvider
    {
        public override string GetWritePassword()
        {
            return "AsposeTestPassword123!";
        }

        // 实现其他必需的方法并返回默认值
        public override string GetOpenPassword() => null;
        public override string GetWorkbookPassword() => null;
        public override ProtectionType GetWorkbookProtectionType() => ProtectionType.None;
        public override string GetWorksheetPassword(string sheetName) => null;
        public override ProtectionType GetWorksheetProtectionType(string sheetName) => ProtectionType.None;
    }
}
```

### 另请参见

* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


