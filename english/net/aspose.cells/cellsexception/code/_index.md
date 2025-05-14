---
title: CellsException.Code
second_title: Aspose.Cells for .NET API Reference
description: CellsException property. Represents custom exception code
type: docs
url: /net/aspose.cells/cellsexception/code/
---
## CellsException.Code property

Represents custom exception code.

```csharp
public ExceptionType Code { get; }
```

### Examples

```csharp
// Called: sb.Append(e.Code);
public static void CellsException_Property_Code(CellsException e, StringBuilder sb)
        {
            sb.Append("CellsException[");
            sb.Append(e.Code);
            sb.Append(": ");
            sb.Append(e.Message);
            sb.Append(']');
        }
```

### See Also

* enum [ExceptionType](../../exceptiontype/)
* class [CellsException](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


