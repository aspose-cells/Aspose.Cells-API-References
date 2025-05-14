---
title: WarningInfo.CorrectedObject
second_title: Aspose.Cells for .NET API Reference
description: WarningInfo property. Gets and sets the corrected object
type: docs
url: /net/aspose.cells/warninginfo/correctedobject/
---
## WarningInfo.CorrectedObject property

Gets and sets the corrected object.

```csharp
public object CorrectedObject { get; set; }
```

### Examples

```csharp
// Called: warningInfo.CorrectedObject = "_" + warningInfo.ErrorObject;
public void WarningInfo_Property_CorrectedObject(WarningInfo warningInfo)
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

* class [WarningInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


