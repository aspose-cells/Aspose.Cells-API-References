---
title: PageSetup.ClearHeaderFooter
second_title: Aspose.Cells for .NET API Reference
description: PageSetup method. Clears header and footer setting
type: docs
url: /net/aspose.cells/pagesetup/clearheaderfooter/
---
## PageSetup.ClearHeaderFooter method

Clears header and footer setting.

```csharp
public void ClearHeaderFooter()
```

### Examples

```csharp
// Called: pageSetup.ClearHeaderFooter();
public void PageSetup_Method_ClearHeaderFooter()
{
    Workbook workbook = new Workbook();
    var pageSetup = workbook.Worksheets[0].PageSetup;

    //This line causes NullReferenceException when setting either Header or Footer below
    pageSetup.ClearHeaderFooter();

    pageSetup.SetHeader(0, "Left Header");
    pageSetup.SetFooter(0, "Left Footer");

            
}
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


