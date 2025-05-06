---
title: CellValue.Type
second_title: Aspose.Cells for .NET API Reference
description: CellValue property. Gets/sets the type of cell value
type: docs
url: /net/aspose.cells/cellvalue/type/
---
## CellValue.Type property

Gets/sets the type of cell value.

```csharp
public CellValueType Type { get; set; }
```

### Examples

```csharp
// Called: value.Type = CellValueType.IsNull;
public override bool Property_Type(int cellRow, int cellColumn, CellValue value)
            {
                if (value.Type == CellValueType.IsError &amp;&amp; &quot;#DIV/0!&quot;.Equals(value.Value))
                {
                    value.Type = CellValueType.IsNull;
                    return true;
                }
                return false;
            }
```

### See Also

* enum [CellValueType](../../cellvaluetype/)
* class [CellValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


