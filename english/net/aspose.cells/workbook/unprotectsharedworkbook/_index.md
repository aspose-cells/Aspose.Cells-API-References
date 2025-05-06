---
title: Workbook.UnprotectSharedWorkbook
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Unprotects a shared workbook
type: docs
url: /net/aspose.cells/workbook/unprotectsharedworkbook/
---
## Workbook.UnprotectSharedWorkbook method

Unprotects a shared workbook.

```csharp
public void UnprotectSharedWorkbook(string password)
```

| Parameter | Type | Description |
| --- | --- | --- |
| password | String | Password to unprotect the workbook. |

### Examples

```csharp
// Called: wb.UnprotectSharedWorkbook(&amp;quot;abcd&amp;quot;);
[Test]
         public void Method_String_()
         {
             Workbook wb = new Workbook();
             wb.ProtectSharedWorkbook(&quot;abcd&quot;);
             wb.Save(Constants.destPath + &quot;ProectSharedWorkbook.xlsx&quot;);
             wb = new Aspose.Cells.Workbook(Constants.destPath + &quot;ProectSharedWorkbook.xlsx&quot;);
             Assert.IsTrue(wb.Settings.IsProtected);
             wb.UnprotectSharedWorkbook(&quot;abcd&quot;);
             wb.Save(Constants.destPath + &quot;UnProectSharedWorkbook.xlsx&quot;);
         }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


