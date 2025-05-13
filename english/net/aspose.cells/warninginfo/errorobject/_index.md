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
// Called: int index = (int)warningInfo.ErrorObject;
public void WarningInfo_Property_ErrorObject(WarningInfo warningInfo)
        {
            switch (warningInfo.Type)
            {
                case ExceptionType.DefinedName:
                    int index = (int)warningInfo.ErrorObject;
                    Name name = wb.Worksheets.Names[index];
                    int index1 = wb.Worksheets.Names.Add(name.Text + "_1");
                    wb.Worksheets.Names[index1].RefersTo = name.RefersTo;
                    warningInfo.CorrectedObject = index1;
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


