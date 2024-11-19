---
title: LoadFilter Class 
linktitle: LoadFilter
second_title: Aspose.Cells for Go API Reference
description: 'LoadFilter class. Encapsulates the object that represents loadfilter in Go.'
type: docs
weight: 200
url: /go/aspose.cells/loadfilter/
---

## LoadFilter class

Represents the filter that provides options for loading data when loading workbook from template.

```go

type LoadFilter struct 

loadfilter, _ := asposecells.NewLoadFilter()

```
## Constructors

| Method | Description |
| --- | --- |
|[NewLoadFilter](./newloadfilter/) | Constructs one LoadFilter with default filter options LoadDataFilterOptions::All. | 
|[NewLoadFilter_LoadDataFilterOptions](./newloadfilter_loaddatafilteroptions/) | Constructs one LoadFilter with given filter options. | 

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[GetLoadDataFilterOptions](./getloaddatafilteroptions/) | Gets the filter options to denote what data should be loaded. | 
|[SetLoadDataFilterOptions](./setloaddatafilteroptions/) | Sets the filter options to denote what data should be loaded. | 
|[StartSheet](./startsheet/) | Prepares filter options before loading given worksheet.User's implementation of LoadFilter can change the LoadDataFilterOptions hereto denote how to load data for this worksheet. | 
