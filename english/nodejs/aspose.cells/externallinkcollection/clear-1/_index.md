---
title: "ExternalLinkCollection.clear"
linktitle: "clear"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Removes all external links."
type: docs
weight: 40
url: /nodejs/aspose.cells/externallinkcollection/clear-1/
---

## clear(updateReferencesAsLocal)

Removes all external links. If references are required to be updated, those references of external links in formulas will be changed to current workbook when it is possible. For example, one cell's original formula is "='externalsource.xlam'!customfunction()", after removing external links, the formula will become "=customfunction()"; When the original formula is "='[externalsource.xlam]Sheet1'!$A$1", according to whether there is one sheet with name "Sheet1" in current workbook: if true, the formula will become "=Sheet1!$A$1"; if false, the formula will become "=#REF!$A$1". If references are not required to be updated, all formulas with references to external links will be removed too because those references become invalid.

| Parameter | Type | Description |
| --- | --- | --- |
| updateReferencesAsLocal | boolean | Whether update all references of external links in formulas to references of current workbook itself. |
