---
title: PageSetup.SetFirstPageHeader
second_title: Aspose.Cells for .NET API Reference
description: PageSetup method. Sets a script formatting the first page header of an Excel file. Only effect in Excel 2007 when IsHFDiffFirst is true
type: docs
url: /net/aspose.cells/pagesetup/setfirstpageheader/
---
## PageSetup.SetFirstPageHeader method

Sets a script formatting the first page header of an Excel file. Only effect in Excel 2007 when IsHFDiffFirst is true.

```csharp
public void SetFirstPageHeader(int section, string headerScript)
```

| Parameter | Type | Description |
| --- | --- | --- |
| section | Int32 | 0: Left Section, 1: Center Section, 2: Right Section. |
| headerScript | String | Header format script. |

### Examples

```csharp
// Called: ps.SetFirstPageHeader(2, "@G");
public void PageSetup_Method_SetFirstPageHeader()
{
    Workbook workbook = new Workbook();
    PageSetup ps = workbook.Worksheets[0].PageSetup;
    byte[] data = File.ReadAllBytes(Constants.sourcePath +"1.jpg");
    ps.SetPicture(true, false, true, 2, data);
    ps.SetFirstPageHeader(2, "@G");
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


