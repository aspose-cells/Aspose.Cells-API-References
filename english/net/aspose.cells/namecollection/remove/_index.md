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
// Called: workbook.Worksheets.Names.Remove("AMB_NUMS");
[Test]
        public void Method_String_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "2007 SF Ranking by KFI Template.xlt");
            workbook.Worksheets.Names.Remove("AMB_NUMS");
            workbook.Save(Constants.destPath +"dest.xls");
        }
```

### See Also

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


