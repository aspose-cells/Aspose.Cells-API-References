---
title: "HtmlTableLoadOptionCollection.Add"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "HtmlTableLoadOptionCollection 方法。向此集合添加一个 HtmlTableLoadOption"
type: docs
url: /zh/net/aspose.cells/htmltableloadoptioncollection/add/
---
## Add(HtmlTableLoadOption) {#add}

向此集合添加一个 HtmlTableLoadOption。

```csharp
[Obsolete("Use HtmlTableLoadOptionCollection.AddTableLoadOption(HtmlTableLoadOption) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(HtmlTableLoadOption item)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 项 | HtmlTableLoadOption | 一个 HtmlTableLoadOption |

### 返回值

已添加 item 的索引

### 备注

注意：此成员已过时。请改用 AddTableLoadOption() 方法。此方法将在自 2025 年 12 月起的 6 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithHtmlTableLoadOptionDemo
    {
        public static void Run()
        {
            // 创建 HTML 加载选项
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // 添加表格加载选项
            HtmlTableLoadOption tableLoadOption1 = new HtmlTableLoadOption();
            tableLoadOption1.Id = "table1";
            loadOptions.TableLoadOptions.Add(tableLoadOption1);

            HtmlTableLoadOption tableLoadOption2 = new HtmlTableLoadOption();
            tableLoadOption2.Id = "table2";
            tableLoadOption2.TargetSheetIndex = 1;
            loadOptions.TableLoadOptions.Add(tableLoadOption2);

            // 加载工作簿并使用选项
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // 保存输出
            workbook.Save("output.xlsx");
        }
    }
}
```

### 另请参见

* class [HtmlTableLoadOption](../../htmltableloadoption/)
* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int) {#add_1}

向列表添加一个 HtmlTableLoadOption。

```csharp
public int Add(int tableIndex)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| tableIndex | Int32 | 表索引 |

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithInt32Demo
    {
        public static void Run()
        {
            // 创建 HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // 访问 HtmlTableLoadOptionCollection 实例
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // 按表索引添加新的 HtmlTableLoadOption
            int index = tableLoadOptions.Add(0);

            // 访问已添加的 HtmlTableLoadOption
            HtmlTableLoadOption option = tableLoadOptions[index];
            option.TableToListObject = true;

            // 创建工作簿并加载带选项的 HTML
            Workbook workbook = new Workbook("input.html", loadOptions);

            // 保存工作簿
            workbook.Save("output.xlsx");
        }
    }
}
```

### 另请参见

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_4}

向列表添加一个 HtmlTableLoadOption。

```csharp
public int Add(string tableId)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| tableId | String | 表 ID |

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            // 创建 HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // 访问 HtmlTableLoadOptionCollection 实例
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // 按表 ID 添加新的 HtmlTableLoadOption
            int index = tableLoadOptions.Add("mainTable");

            // 访问已添加的 HtmlTableLoadOption
            HtmlTableLoadOption option = tableLoadOptions[index];
            option.TableToListObject = true;
            option.TargetSheetIndex = 0;

            // 创建工作簿并加载带选项的 HTML
            Workbook workbook = new Workbook("input.html", loadOptions);

            // 保存工作簿
            workbook.Save("output.xlsx");
        }
    }
}
```

### 另请参见

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int) {#add_2}

向列表添加一个 HtmlTableLoadOption。

```csharp
public int Add(int tableIndex, int targetSheetIndex)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| tableIndex | Int32 | 表索引 |
| targetSheetIndex | Int32 | Excel 中 worksheet 的目标索引 |

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // 创建 HTML 加载选项
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // 按索引添加表，并使用目标工作表索引
            loadOptions.TableLoadOptions.Add(0, 2); // Table index 0 to sheet index 2
            loadOptions.TableLoadOptions.Add(1, 0); // Table index 1 to sheet index 0
            loadOptions.TableLoadOptions.Add(2, 1); // Table index 2 to sheet index 1

            // 使用指定选项加载 HTML 文件
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // 保存工作簿
            workbook.Save("output.xlsx");
        }
    }
}
```

### 另请参见

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int) {#add_5}

向列表添加一个 HtmlTableLoadOption。

```csharp
public int Add(string tableId, int targetSheetIndex)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| tableId | String | 表 ID |
| targetSheetIndex | Int32 | Excel 中 worksheet 的目标索引 |

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithStringInt32Demo
    {
        public static void Run()
        {
            // 创建 HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // 访问 HtmlTableLoadOptionCollection 实例
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // 按表 ID 和目标工作表索引添加新的 HtmlTableLoadOption
            int index = tableLoadOptions.Add("tableId", 1);

            // 创建工作簿并加载带选项的 HTML
            Workbook workbook = new Workbook("input.html", loadOptions);

            // 保存工作簿
            workbook.Save("output.xlsx");
        }
    }
}
```

### 另请参见

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, int) {#add_3}

向列表添加一个 HtmlTableLoadOption。

```csharp
public int Add(int tableIndex, int targetSheetIndex, int originalSheetIndex)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| tableIndex | Int32 | 表索引 |
| targetSheetIndex | Int32 | Excel 中 worksheet 的目标索引 |
| originalSheetIndex | Int32 | HTML 中 worksheet 的原始索引 |

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // 创建 HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // 访问 HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // 添加一个表，索引为 1，目标工作表索引为 1，原始工作表索引为 0
            int addedIndex = tableLoadOptions.Add(1, 1, 0);

            // 创建工作簿并加载带选项的 HTML
            Workbook workbook = new Workbook("input.html", loadOptions);

            // 保存结果
            workbook.Save("output.xlsx");
        }
    }
}
```

### 另请参见

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int) {#add_6}

向列表添加一个 HtmlTableLoadOption。

```csharp
public int Add(string tableId, int targetSheetIndex, int originalSheetIndex)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| tableId | String | 表 ID |
| targetSheetIndex | Int32 | Excel 中 worksheet 的目标索引 |
| originalSheetIndex | Int32 | HTML 中 worksheet 的原始索引 |

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionCollectionMethodAddWithStringInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // 演示使用 (String, Int32, Int32) 参数的 Add 方法
            int addedIndex = tableLoadOptions.Add("sampleTable", 1, 0);
            
            HtmlTableLoadOption option = tableLoadOptions[addedIndex];
            option.TableToListObject = true;

            // 加载 HTML 文件（请替换为实际文件路径）
            workbook = new Workbook("input.html", loadOptions);
            workbook.Save("output.xlsx");
        }
    }
}
```

### 另请参见

* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


