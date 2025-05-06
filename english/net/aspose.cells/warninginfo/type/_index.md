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
public void Property_Type(WarningInfo warningInfo)
        {
            switch (warningInfo.Type)
            {
                case ExceptionType.DefinedName:
                    int index = (int)warningInfo.ErrorObject;
                    Name name = wb.Worksheets.Names[index];
                    int index1 = wb.Worksheets.Names.Add(name.Text + &quot;_1&quot;);
                    wb.Worksheets.Names[index1].RefersTo = name.RefersTo;
                    warningInfo.CorrectedObject = index1;
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


