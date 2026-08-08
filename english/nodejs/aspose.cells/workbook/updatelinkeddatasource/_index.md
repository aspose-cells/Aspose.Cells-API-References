---
title: "Workbook.updateLinkedDataSource"
linktitle: "updateLinkedDataSource"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "If this workbook contains external links to other data source, Aspose.Cells will attempt to retrieve the latest data from give sources."
type: docs
weight: 950
url: /nodejs/aspose.cells/workbook/updatelinkeddatasource/
---

## updateLinkedDataSource(externalWorkbooks)

If this workbook contains external links to other data source, Aspose.Cells will attempt to retrieve the latest data from give sources. If corresponding external link cannot be found for one workbook, then this workbook will be ignored. So when you set a formula later with one new external link which you intend to make the ignored workbook be linked to it, the link cannot be performed until you call this this method again with those workbooks.

| Parameter | Type | Description |
| --- | --- | --- |
| externalWorkbooks | Array ofWorkbook | Workbooks that will be used to update data of external links referenced by this workbook. The match of those workbooks with external links is determined by |
