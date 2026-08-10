---
title: "CopyOptions Class"
linktitle: "CopyOptions"
articleTitle: "CopyOptions"
second_title: "Aspose.Cells for Python via Java"
description: "Represents the copy options."
type: docs
weight: 1340
url: /python-java/asposecells.api/copyoptions/
---

## CopyOptions class

Represents the copy options.

## Constructors

| Name | Description |
| --- | --- |
| [CopyOptions](#constructor) | CopyOptions constructor. |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [KeepMacros](#keepmacros) | boolean | Indicates whether keeping macros; Only for copying workbook. |
| [ExtendToAdjacentRange](#extendtoadjacentrange) | boolean | Indicates whether extend ranges when copying the range to adjacent range. If it's true, only extends the range of the hy |
| [CopyNames](#copynames) | boolean | Indicates whether copying the names. |
| [CopyInvalidFormulasAsValues](#copyinvalidformulasasvalues) | boolean | If the formula is not valid for the dest destination, only copy values. |
| [ColumnCharacterWidth](#columncharacterwidth) | boolean | Indicates whether copying column width in unit of characters. |
| [ReferToSheetWithSameName](#refertosheetwithsamename) | boolean | In ms excel, when copying formulas which refer to other worksheets while copying a worksheet to another one, the copied  |
| [ReferToDestinationSheet](#refertodestinationsheet) | boolean | When copying the range in the same file and the chart refers to the source sheet, False means the copied chart's data so |
| [UpdateInvalidReferencesToTargetSheet](#updateinvalidreferencestotargetsheet) | boolean |  |

### CopyOptions() {#constructor}

CopyOptions constructor.

### CopyOptions.KeepMacros property {#keepmacros}

Indicates whether keeping macros; Only for copying workbook.

**Type:** boolean

### CopyOptions.ExtendToAdjacentRange property {#extendtoadjacentrange}

Indicates whether extend ranges when copying the range to adjacent range. If it's true, only extends the range of the hyperlink,not adding a new hyperlink when copying hyperlinks to adjacent rows.

**Type:** boolean

### CopyOptions.CopyNames property {#copynames}

Indicates whether copying the names.

**Type:** boolean

### CopyOptions.CopyInvalidFormulasAsValues property {#copyinvalidformulasasvalues}

If the formula is not valid for the dest destination, only copy values.

**Type:** boolean

### CopyOptions.ColumnCharacterWidth property {#columncharacterwidth}

Indicates whether copying column width in unit of characters.

**Type:** boolean

### CopyOptions.ReferToSheetWithSameName property {#refertosheetwithsamename}

In ms excel, when copying formulas which refer to other worksheets while copying a worksheet to another one, the copied formulas should refer to source workbook. However, for some situations user may need the copied formulas refer to worksheets with the same name in the same workbook, such as when those worksheets have been copied before this copy operation, then this property should be kept as true. The default value is true.

**Type:** boolean

### CopyOptions.ReferToDestinationSheet property {#refertodestinationsheet}

When copying the range in the same file and the chart refers to the source sheet, False means the copied chart's data source will not be changed. True means the copied chart's data source refers to the destination sheet. The default value is false, it works as MS Excel.

**Type:** boolean

### CopyOptions.UpdateInvalidReferencesToTargetSheet property {#updateinvalidreferencestotargetsheet}

**Type:** boolean
