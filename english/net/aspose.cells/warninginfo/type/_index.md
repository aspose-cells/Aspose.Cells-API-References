---
title: WarningInfo.Type
second_title: Aspose.Cells for .NET API Reference
description: WarningInfo property. Get warning type
type: docs
url: /net/aspose.cells/warninginfo/type/
---
## WarningInfo.Type property

Get warning type.

```csharp
public ExceptionType Type { get; }
```

### Examples

```csharp
// Called: switch (warningInfo.Type)
public void WarningInfo_Property_Type(WarningInfo warningInfo)
        {
            switch (warningInfo.Type)
            {
                case ExceptionType.DefinedName:
                    warningInfo.CorrectedObject = "_" + warningInfo.ErrorObject;
                    return;
                case ExceptionType.Font:
                // throw new CellsException(ExceptionType.InvalidData, warningInfo.Description);
                case ExceptionType.FileFormat:
                // throw new CellsException(ExceptionType.UnsupportedStream, "Unsupported file format.");
                case ExceptionType.IO:
                case ExceptionType.InvalidData:
                case ExceptionType.Limitation:
                    return;
                default:
                    break;
            }
        }
```

### See Also

* enum [ExceptionType](../../exceptiontype/)
* class [WarningInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


