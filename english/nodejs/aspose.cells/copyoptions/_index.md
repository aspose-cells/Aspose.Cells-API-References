---
title: "CopyOptions"
linktitle: "CopyOptions"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents the copy options."
type: docs
weight: 870
url: /nodejs/aspose.cells/copyoptions/
---

## CopyOptions class

Represents the copy options.

```js
new CopyOptions()
```

CopyOptions constructor.

## Methods

| Name | Description |
| --- | --- |
| [getColumnCharacterWidth()](#getcolumncharacterwidth) | Indicates whether copying column width in unit of characters. |
| [getCopyInvalidFormulasAsValues()](#getcopyinvalidformulasasvalues) | If the formula is not valid for the dest destination, only copy values. |
| [getCopyNames()](#getcopynames) | Indicates whether copying the names. |
| [getExtendToAdjacentRange()](#getextendtoadjacentrange) | Indicates whether extend ranges when copying the range to adjacent range. If it's true, only extends the range of the hy |
| [getKeepMacros()](#getkeepmacros) | Indicates whether keeping macros; Only for copying workbook. |
| [getReferToDestinationSheet()](#getrefertodestinationsheet) | When copying the range in the same file and the chart refers to the source sheet, False means the copied chart's data so |
| [getReferToSheetWithSameName()](#getrefertosheetwithsamename) | In ms excel, when copying formulas which refer to other worksheets while copying a worksheet to another one, the copied  |
| [getUpdateInvalidReferencesToTargetSheet()](#getupdateinvalidreferencestotargetsheet) |  |
| [setColumnCharacterWidth()](#setcolumncharacterwidth) | Indicates whether copying column width in unit of characters. |
| [setCopyInvalidFormulasAsValues()](#setcopyinvalidformulasasvalues) | If the formula is not valid for the dest destination, only copy values. |
| [setCopyNames()](#setcopynames) | Indicates whether copying the names. |
| [setExtendToAdjacentRange()](#setextendtoadjacentrange) | Indicates whether extend ranges when copying the range to adjacent range. If it's true, only extends the range of the hy |
| [setKeepMacros()](#setkeepmacros) | Indicates whether keeping macros; Only for copying workbook. |
| [setReferToDestinationSheet()](#setrefertodestinationsheet) | When copying the range in the same file and the chart refers to the source sheet, False means the copied chart's data so |
| [setReferToSheetWithSameName()](#setrefertosheetwithsamename) | In ms excel, when copying formulas which refer to other worksheets while copying a worksheet to another one, the copied  |
| [setUpdateInvalidReferencesToTargetSheet()](#setupdateinvalidreferencestotargetsheet) |  |

### getColumnCharacterWidth() {#getcolumncharacterwidth}

Indicates whether copying column width in unit of characters.

### getCopyInvalidFormulasAsValues() {#getcopyinvalidformulasasvalues}

If the formula is not valid for the dest destination, only copy values.

### getCopyNames() {#getcopynames}

Indicates whether copying the names.

### getExtendToAdjacentRange() {#getextendtoadjacentrange}

Indicates whether extend ranges when copying the range to adjacent range. If it's true, only extends the range of the hyperlink,not adding a new hyperlink when copying hyperlinks to adjacent rows.

### getKeepMacros() {#getkeepmacros}

Indicates whether keeping macros; Only for copying workbook.

### getReferToDestinationSheet() {#getrefertodestinationsheet}

When copying the range in the same file and the chart refers to the source sheet, False means the copied chart's data source will not be changed. True means the copied chart's data source refers to the destination sheet. The default value is false, it works as MS Excel.

### getReferToSheetWithSameName() {#getrefertosheetwithsamename}

In ms excel, when copying formulas which refer to other worksheets while copying a worksheet to another one, the copied formulas should refer to source workbook. However, for some situations user may need the copied formulas refer to worksheets with the same name in the same workbook, such as when those worksheets have been copied before this copy operation, then this property should be kept as true. The default value is true.

### getUpdateInvalidReferencesToTargetSheet() {#getupdateinvalidreferencestotargetsheet}

### setColumnCharacterWidth() {#setcolumncharacterwidth}

Indicates whether copying column width in unit of characters.

### setCopyInvalidFormulasAsValues() {#setcopyinvalidformulasasvalues}

If the formula is not valid for the dest destination, only copy values.

### setCopyNames() {#setcopynames}

Indicates whether copying the names.

### setExtendToAdjacentRange() {#setextendtoadjacentrange}

Indicates whether extend ranges when copying the range to adjacent range. If it's true, only extends the range of the hyperlink,not adding a new hyperlink when copying hyperlinks to adjacent rows.

### setKeepMacros() {#setkeepmacros}

Indicates whether keeping macros; Only for copying workbook.

### setReferToDestinationSheet() {#setrefertodestinationsheet}

When copying the range in the same file and the chart refers to the source sheet, False means the copied chart's data source will not be changed. True means the copied chart's data source refers to the destination sheet. The default value is false, it works as MS Excel.

### setReferToSheetWithSameName() {#setrefertosheetwithsamename}

In ms excel, when copying formulas which refer to other worksheets while copying a worksheet to another one, the copied formulas should refer to source workbook. However, for some situations user may need the copied formulas refer to worksheets with the same name in the same workbook, such as when those worksheets have been copied before this copy operation, then this property should be kept as true. The default value is true.

### setUpdateInvalidReferencesToTargetSheet() {#setupdateinvalidreferencestotargetsheet}
