---
title: "Chart.isChartDataChanged"
linktitle: "isChartDataChanged"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Detects if a chart's data source has changed."
type: docs
weight: 600
url: /nodejs/aspose.cells/chart/ischartdatachanged/
---

## isChartDataChanged()

Detects if a chart's data source has changed. The method detects the changes in the chart's data source before rendering the chart to image format. At first Chart.toImage call, the chart source data (e.g. XValuesParseData, ValuesParseData) will be recorded. Before calling the Chart.toImage method again, call IsChartDataChanged method to check if Chart needs re-rendering.

**Returns:** boolean — `boolean` Returns true if the chart has changed otherwise returns false
