---
title: "VbaModuleCollection.AddUserForm"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "VbaModuleCollection 方法。将用户窗体插入 VBA 项目"
type: docs
url: /zh/net/aspose.cells.vba/vbamodulecollection/adduserform/
---
## VbaModuleCollection.AddUserForm method

将用户窗体插入 VBA 项目。

```csharp
public int AddUserForm(string name, string codes, byte[] designerStorage)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | String | 用户窗体的名称 |
| 代码 | String | 用户窗体的代码 |
| designerStorage | Byte[] | 关于用户窗体的设计器设置 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;
    using System.IO;

    public class VbaModuleCollectionMethodAddUserFormWithStringStringByteDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 访问 VBA 项目
            VbaProject vbaProject = workbook.VbaProject;
            VbaModuleCollection vbaModules = vbaProject.Modules;

            // 准备 AddUserForm 的参数
            string formName = "UserForm1";
            string formCode = 
                "Private Sub CommandButton1_Click()\n" +
                "    MsgBox \"Hello from UserForm!\"\n" +
                "End Sub";
            
            // 创建一个简单的设计器存储（这通常是 .frx 二进制数据）
            byte[] designerStorage = new byte[] { 0x00, 0x01, 0x02, 0x03 };

            try
            {
                // 使用 (String, String, Byte[]) 参数调用 AddUserForm
                int moduleIndex = vbaModules.AddUserForm(formName, formCode, designerStorage);
                
                Console.WriteLine($"UserForm added successfully at index: {moduleIndex}");
                Console.WriteLine($"Total VBA modules: {vbaModules.Count}");

                // 保存工作簿以查看 VBA 项目更改
                workbook.Save("AddUserFormDemo.xlsm", SaveFormat.Xlsm);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding UserForm: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


