---
title: OoxmlSaveOptions.EmbedOoxmlAsOleObject
second_title: Aspose.Cells for .NET API Reference
description: OoxmlSaveOptions property. Indicates whether embedding Ooxml files of OleObject as ole object
type: docs
url: /net/aspose.cells/ooxmlsaveoptions/embedooxmlasoleobject/
---
## OoxmlSaveOptions.EmbedOoxmlAsOleObject property

Indicates whether embedding Ooxml files of OleObject as ole object.

```csharp
public bool EmbedOoxmlAsOleObject { get; set; }
```

### Remarks

Only for OleObject.

### Examples

```csharp
// Called: saveOptions.EmbedOoxmlAsOleObject = true;
[Test]
        public void Property_EmbedOoxmlAsOleObject()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET46712.xls");
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.EmbedOoxmlAsOleObject = true;
            workbook.Save(Constants.destPath + "CELLSNET46714.xlsx", saveOptions);
        }
```

### See Also

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


