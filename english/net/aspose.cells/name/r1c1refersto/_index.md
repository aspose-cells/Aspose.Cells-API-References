---
title: Name.R1C1RefersTo
second_title: Aspose.Cells for .NET API Reference
description: Name property. Gets or sets a R1C1 reference of the Name
type: docs
url: /net/aspose.cells/name/r1c1refersto/
---
## Name.R1C1RefersTo property

Gets or sets a R1C1 reference of the [`Name`](../).

```csharp
public string R1C1RefersTo { get; set; }
```

### Examples

```csharp
// Called: name.R1C1RefersTo = &amp;quot;=Sheet1!R2C10&amp;quot;;
[Test]
        public void Property_R1C1RefersTo()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Names.Add(&quot;test&quot;);
           Name name =  workbook.Worksheets.Names[0];
           name.R1C1RefersTo = &quot;=Sheet1!R2C10&quot;;
           workbook.Save(Constants.destPath + &quot;Test_199623.xls&quot;);


        }
```

### See Also

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


