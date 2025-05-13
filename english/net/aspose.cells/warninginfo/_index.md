---
title: Class WarningInfo
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.WarningInfo class. Warning info
type: docs
url: /net/aspose.cells/warninginfo/
---
## WarningInfo class

Warning info

```csharp
public class WarningInfo
```

## Properties

| Name | Description |
| --- | --- |
| [CorrectedObject](../../aspose.cells/warninginfo/correctedobject/) { get; set; } | Gets and sets the corrected object. |
| [Description](../../aspose.cells/warninginfo/description/) { get; } | Get description of warning info. |
| [ErrorObject](../../aspose.cells/warninginfo/errorobject/) { get; } | The error object. |
| [Type](../../aspose.cells/warninginfo/type/) { get; } | Get warning type. |
| [WarningType](../../aspose.cells/warninginfo/warningtype/) { get; } | (**Obsolete.**) Get warning type. |

### Examples

```csharp
// Called: public void Warning(WarningInfo warningInfo)
public void Cells_Type_WarningInfo(WarningInfo warningInfo)
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

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


