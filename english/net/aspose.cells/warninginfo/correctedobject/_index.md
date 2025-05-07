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
// Called: warningInfo.CorrectedObject = index1;
public void Property_CorrectedObject(WarningInfo warningInfo)
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


