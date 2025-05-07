---
title: Style.Update
second_title: Aspose.Cells for .NET API Reference
description: Style method. Apply the named style to the styles of the cells which use this named style. It works like clicking the ok button after you finished modifying the style. Only applies for named style
type: docs
url: /net/aspose.cells/style/update/
---
## Style.Update method

Apply the named style to the styles of the cells which use this named style. It works like clicking the "ok" button after you finished modifying the style. Only applies for named style.

```csharp
public void Update()
```

### Examples

```csharp
// Called: style.Update();
[Test]
        public void Method_Update()
        {
            Workbook workbook = new Workbook();
            Style style = workbook.GetNamedStyle("Normal");
            style.Font.Name = "Tahoma";
            style.Font.Size = 11;
            style.VerticalAlignment = TextAlignmentType.Top;
            style.Update();
            workbook.Save(Constants.destPath + "TestDefaultStyle.xls");

        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


