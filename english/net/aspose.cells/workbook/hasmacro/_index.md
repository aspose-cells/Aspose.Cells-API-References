---
title: Workbook.HasMacro
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Indicates if this spreadsheet contains macro/VBA
type: docs
url: /net/aspose.cells/workbook/hasmacro/
---
## Workbook.HasMacro property

Indicates if this spreadsheet contains macro/VBA.

```csharp
public bool HasMacro { get; }
```

### Examples

```csharp
// Called: Console.WriteLine("is workbook has macro :" + workbook.HasMacro);
public void Workbook_Property_HasMacro()
{
    // http://www.aspose.com/community/forums/thread/211124.aspx
    Console.WriteLine("Workbook_Property_HasMacro()");
    string infn = path + "Test_HasMacro.xlsm";

    Workbook workbook = new Workbook(infn);
    Console.WriteLine("is workbook has macro :" + workbook.HasMacro);
}
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


