---
title: "RenameStrategy"
linktitle: "RenameStrategy"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Utility class containing constants."
type: docs
weight: 2180
url: /nodejs/global/renamestrategy/
---

## RenameStrategy

Utility class containing constants. Strategy option for duplicate names of columns. When processing data with headers, some scenarios require the headers to be no duplication for all columns. For example, when exporting data to a datatable and the header is required to be taken as datatable's column name, duplicated values of the header are invalid. For such kind of situations, user may determine how to handle them by specifying this strategy.

## Values

| Name | Description |
| --- | --- |
| EXCEPTION | Throws exception. |
| DIGIT | Named with digit. Duplicated names will become ...1, ...2, etc. |
| LETTER | Named with letter.. Duplicated names will become ...A, ...B, etc. |
