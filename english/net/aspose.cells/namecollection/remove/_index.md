---
title: NameCollection.Remove
second_title: Aspose.Cells for .NET API Reference
description: NameCollection method. Remove an array of name
type: docs
url: /net/aspose.cells/namecollection/remove/
---
## Remove(string[]) {#remove_1}

Remove an array of name

```csharp
public void Remove(string[] names)
```

| Parameter | Type | Description |
| --- | --- | --- |
| names | String[] | The names' text. |

### See Also

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Remove(string) {#remove}

Remove the name.

```csharp
public void Remove(string text)
```

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | The name text. |

### Examples

```csharp
// Called: workbook.Worksheets.Names.Remove("Source!EHC_Admin");
public void NameCollection_Method_Remove()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    int count = workbook.Worksheets.Names.Count;
    //workbook.Worksheets.DeleteName("Source!EHC_Admin");
    workbook.Worksheets.Names.Remove("Source!EHC_Admin");
    Worksheet sheet = workbook.Worksheets["Test"];
    Aspose.Cells.Range range = sheet.Cells.CreateRange("A1", "B10");

    range.Name = "EHC_Admin";
    Assert.AreEqual(workbook.Worksheets.Names.Count, count);
    workbook.Save(Constants.destPath + "example.xls");
}
```

### See Also

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


