---
title: GetEnumerator
second_title: Aspose.Cells for .NET API 参考
description: 获取单元格 enumerator
type: docs
weight: 180
url: /zh/net/aspose.cells/row/getenumerator/
---
## Row.GetEnumerator method

获取单元格 enumerator

```csharp
public IEnumerator GetEnumerator()
```

### 返回值

单元格枚举器

### 例子

```csharp
[C#]
Workbook workbook = new Workbook("template.xlsx");
Cells cells = workbook.Worksheets[0].Cells;

IEnumerator en = cells.Rows[1].GetEnumerator();
while (en.MoveNext())
{
    Cell cell = (Cell)en.Current;
    Console.WriteLine(cell.Name + ": " + cell.Value);
}
```

### 也可以看看

* class [Row](../../row)
* 命名空间 [Aspose.Cells](../../row)
* 部件 [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
