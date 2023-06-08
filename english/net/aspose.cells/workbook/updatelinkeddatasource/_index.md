---
title: Workbook.UpdateLinkedDataSource
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. If this workbook contains external links to other data source Aspose.Cells will attempt to retrieve the latest data from give sources
type: docs
url: /net/aspose.cells/workbook/updatelinkeddatasource/
---
## Workbook.UpdateLinkedDataSource method

If this workbook contains external links to other data source, Aspose.Cells will attempt to retrieve the latest data from give sources.

```csharp
public void UpdateLinkedDataSource(Workbook[] externalWorkbooks)
```

| Parameter | Type | Description |
| --- | --- | --- |
| externalWorkbooks | Workbook[] | Workbooks that will be used to update data of external links referenced by this workbook. The match of those workbooks with external links is determined by [`FileName`](../filename/) and [`DataSource`](../../externallink/datasource/). So please make sure [`FileName`](../filename/) has been specified with the proper value for every workbook so they can be linked to corresponding external link. |

### Remarks

If corresponding external link cannot be found for one workbook, then this workbook will be ignored. So when you set a formula later with one new external link which you intend to make the ignored workbook be linked to it, the link cannot be performed until you call this this method again with those workbooks.

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


