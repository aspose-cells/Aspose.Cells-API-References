---
title: WarningInfo.ErrorObject
second_title: Aspose.Cells for .NET API Reference
description: WarningInfo property. The error object
type: docs
url: /net/aspose.cells/warninginfo/errorobject/
---
## WarningInfo.ErrorObject property

The error object.

```csharp
public object ErrorObject { get; }
```

### Examples

```csharp
// Called: warningInfo.CorrectedObject = "_" + warningInfo.ErrorObject;
public void Property_ErrorObject(WarningInfo warningInfo)
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
                        //Console.WriteLine(warningInfo.Description);
                        return;
                    case ExceptionType.InvalidData:
                    case ExceptionType.Limitation:
                        return;
                    default:
                        break;
                }
            }
```

### See Also

* class [WarningInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


