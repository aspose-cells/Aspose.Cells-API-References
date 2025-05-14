---
title: XlsSaveOptions.IsTemplate
second_title: Aspose.Cells for .NET API Reference
description: XlsSaveOptions property. Indicates whether saving a template file
type: docs
url: /net/aspose.cells/xlssaveoptions/istemplate/
---
## XlsSaveOptions.IsTemplate property

Indicates whether saving a template file.

```csharp
[Obsolete("Use XlsSaveOptions(SaveFormat.Xlt) when it is template, otherwise use XlsSaveOptions().")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsTemplate { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please create XlsSaveOptions with corresponding save format(xlt for true and xls for false). This method will be removed 12 months later since August 2020. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: saveOptions.IsTemplate = true;
public void XlsSaveOptions_Property_IsTemplate()
{
    Workbook workbook = new Workbook();
    using (FileStream fs = File.Create(Constants.destPath + "Xlt001"))
    {
        XlsSaveOptions saveOptions = new XlsSaveOptions();
        saveOptions.IsTemplate = true;
        workbook.Save(fs, saveOptions);
    }
    workbook = new Workbook(Constants.destPath + "Xlt001");
    Assert.AreEqual(workbook.FileFormat, FileFormatType.Xlt);
}
```

### See Also

* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


