---
title: RegisterAddInFunction
second_title: Aspose.Cells for .NET API 参考
description: 将插件函数添加到工作簿
type: docs
weight: 290
url: /zh/net/aspose.cells/worksheetcollection/registeraddinfunction/
---
## RegisterAddInFunction(string, string, bool) {#registeraddinfunction}

将插件函数添加到工作簿

```csharp
public int RegisterAddInFunction(string addInFile, string functionName, bool lib)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| addInFile | String | 文件包含插件函数 |
| functionName | String | 插件函数名 |
| lib | Boolean | 给定的插件文件是否在工作簿加载项库的目录或子目录。 当给定 addInFile 是相对路径时，此标志生效并有所不同: true 表示路径相对于加载项库，false 表示路径相对于此工作簿. |

### 返回值

包含给定插件函数的数据的 ID

### 也可以看看

* class [WorksheetCollection](../../worksheetcollection)
* 命名空间 [Aspose.Cells](../../worksheetcollection)
* 部件 [Aspose.Cells](../../../)

---

## RegisterAddInFunction(int, string) {#registeraddinfunction_1}

将插件函数添加到工作簿

```csharp
public string RegisterAddInFunction(int id, string functionName)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| id | Int32 | 数据的 ID其中包含插件函数， 可以通过[`RegisterAddInFunction`](../registeraddinfunction)的第一次调用获得对于相同的插件文件。 |
| functionName | String | 插件函数名称 |

### 返回值

包含插件函数的插件文件的 URL

### 也可以看看

* class [WorksheetCollection](../../worksheetcollection)
* 命名空间 [Aspose.Cells](../../worksheetcollection)
* 部件 [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->