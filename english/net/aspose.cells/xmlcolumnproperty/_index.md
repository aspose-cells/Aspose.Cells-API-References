---
title: Class XmlColumnProperty
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.XmlColumnProperty class. Represents Xml Data Binding information
type: docs
url: /net/aspose.cells/xmlcolumnproperty/
---
## XmlColumnProperty class

Represents Xml Data Binding information.

```csharp
public class XmlColumnProperty
```

## Constructors

| Name | Description |
| --- | --- |
| [XmlColumnProperty](xmlcolumnproperty/)() | The default constructor. |

### Examples

```csharp
[C#]

namespace Demos
{
    using Aspose.Cells;
    using System;

    public class XmlColumnPropertyDemo
    {
        public static void XmlColumnPropertyExample()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access the first worksheet in the workbook
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Create an instance of XmlColumnProperty
            XmlColumnProperty xmlColumnProperty = new XmlColumnProperty();
            
            // Since XmlColumnProperty does not have any properties or methods,
            // we will just demonstrate creating an instance of it.
            
            // Save the workbook
            workbook.Save("XmlColumnPropertyExample.xlsx");

            return;
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


