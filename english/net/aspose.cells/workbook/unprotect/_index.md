---
title: Workbook.Unprotect
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Unprotects a workbook
type: docs
url: /net/aspose.cells/workbook/unprotect/
---
## Workbook.Unprotect method

Unprotects a workbook.

```csharp
public void Unprotect(string password)
```

| Parameter | Type | Description |
| --- | --- | --- |
| password | String | Password to unprotect the workbook. |

### Examples

```csharp
// Called: workbook.Unprotect(&amp;quot;book&amp;quot;); // Correct password is &amp;quot;book&amp;quot;
[Test]
        public void Method_String_()
        {
            LoadOptions lo = new LoadOptions() { Password = &quot;excel&quot; };
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet45534.xlsx&quot;, lo);
            workbook.Unprotect(&quot;book&quot;); // Correct password is &quot;book&quot;
            workbook.Save(Constants.destPath + &quot;CellsNet45534.xlsx&quot;);
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


