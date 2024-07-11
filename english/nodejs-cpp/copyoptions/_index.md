---
title: CopyOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the copy options.
type: docs
url: /nodejs-cpp/copyoptions/
---

## CopyOptions class

Represents the copy options.

```javascript
class CopyOptions;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| CopyOptions constructor. |

## Methods

| Method | Description |
| --- | --- |
| [getKeepMacros()](#getKeepMacros--)| Indicates whether keeping macros; |
| [setKeepMacros(boolean)](#setKeepMacros-boolean-)| Indicates whether keeping macros; |
| [getExtendToAdjacentRange()](#getExtendToAdjacentRange--)| Indicates whether extend ranges when copying the range to adjacent range. |
| [setExtendToAdjacentRange(boolean)](#setExtendToAdjacentRange-boolean-)| Indicates whether extend ranges when copying the range to adjacent range. |
| [getCopyNames()](#getCopyNames--)| Indicates whether copying the names. |
| [setCopyNames(boolean)](#setCopyNames-boolean-)| Indicates whether copying the names. |
| [getCopyInvalidFormulasAsValues()](#getCopyInvalidFormulasAsValues--)| If the formula is not valid for the dest destination, only copy values. |
| [setCopyInvalidFormulasAsValues(boolean)](#setCopyInvalidFormulasAsValues-boolean-)| If the formula is not valid for the dest destination, only copy values. |
| [getColumnCharacterWidth()](#getColumnCharacterWidth--)| Indicates whether copying column width in unit of characters. |
| [setColumnCharacterWidth(boolean)](#setColumnCharacterWidth-boolean-)| Indicates whether copying column width in unit of characters. |
| [getReferToSheetWithSameName()](#getReferToSheetWithSameName--)| In ms excel, when copying formulas which refer to other worksheets while copying a worksheet to another one, the copied formulas should refer to source workbook. However, for some situations user may need the copied formulas refer to worksheets with the same name in the same workbook, such as when those worksheets have been copied before this copy operation, then this property should be kept as true. |
| [setReferToSheetWithSameName(boolean)](#setReferToSheetWithSameName-boolean-)| In ms excel, when copying formulas which refer to other worksheets while copying a worksheet to another one, the copied formulas should refer to source workbook. However, for some situations user may need the copied formulas refer to worksheets with the same name in the same workbook, such as when those worksheets have been copied before this copy operation, then this property should be kept as true. |
| [getReferToDestinationSheet()](#getReferToDestinationSheet--)| When copying the range in the same file and the chart refers to the source sheet, False means the copied chart's data source will not be changed. True means the copied chart's data source refers to the destination sheet. |
| [setReferToDestinationSheet(boolean)](#setReferToDestinationSheet-boolean-)| When copying the range in the same file and the chart refers to the source sheet, False means the copied chart's data source will not be changed. True means the copied chart's data source refers to the destination sheet. |


### constructor() {#constructor--}

CopyOptions constructor.

```javascript
constructor();
```


### getKeepMacros() {#getKeepMacros--}

Indicates whether keeping macros;

```javascript
getKeepMacros() : boolean;
```


**Remarks**

Only for copying workbook.

### setKeepMacros(boolean) {#setKeepMacros-boolean-}

Indicates whether keeping macros;

```javascript
setKeepMacros(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Only for copying workbook.

### getExtendToAdjacentRange() {#getExtendToAdjacentRange--}

Indicates whether extend ranges when copying the range to adjacent range.

```javascript
getExtendToAdjacentRange() : boolean;
```


**Remarks**

If it's true, only extends the range of the hyperlink,not adding a new hyperlink when copying hyperlinks to adjacent rows.

### setExtendToAdjacentRange(boolean) {#setExtendToAdjacentRange-boolean-}

Indicates whether extend ranges when copying the range to adjacent range.

```javascript
setExtendToAdjacentRange(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

If it's true, only extends the range of the hyperlink,not adding a new hyperlink when copying hyperlinks to adjacent rows.

### getCopyNames() {#getCopyNames--}

Indicates whether copying the names.

```javascript
getCopyNames() : boolean;
```


### setCopyNames(boolean) {#setCopyNames-boolean-}

Indicates whether copying the names.

```javascript
setCopyNames(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getCopyInvalidFormulasAsValues() {#getCopyInvalidFormulasAsValues--}

If the formula is not valid for the dest destination, only copy values.

```javascript
getCopyInvalidFormulasAsValues() : boolean;
```


### setCopyInvalidFormulasAsValues(boolean) {#setCopyInvalidFormulasAsValues-boolean-}

If the formula is not valid for the dest destination, only copy values.

```javascript
setCopyInvalidFormulasAsValues(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getColumnCharacterWidth() {#getColumnCharacterWidth--}

Indicates whether copying column width in unit of characters.

```javascript
getColumnCharacterWidth() : boolean;
```


### setColumnCharacterWidth(boolean) {#setColumnCharacterWidth-boolean-}

Indicates whether copying column width in unit of characters.

```javascript
setColumnCharacterWidth(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getReferToSheetWithSameName() {#getReferToSheetWithSameName--}

In ms excel, when copying formulas which refer to other worksheets while copying a worksheet to another one, the copied formulas should refer to source workbook. However, for some situations user may need the copied formulas refer to worksheets with the same name in the same workbook, such as when those worksheets have been copied before this copy operation, then this property should be kept as true.

```javascript
getReferToSheetWithSameName() : boolean;
```


**Remarks**

The default value is true.

### setReferToSheetWithSameName(boolean) {#setReferToSheetWithSameName-boolean-}

In ms excel, when copying formulas which refer to other worksheets while copying a worksheet to another one, the copied formulas should refer to source workbook. However, for some situations user may need the copied formulas refer to worksheets with the same name in the same workbook, such as when those worksheets have been copied before this copy operation, then this property should be kept as true.

```javascript
setReferToSheetWithSameName(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

The default value is true.

### getReferToDestinationSheet() {#getReferToDestinationSheet--}

When copying the range in the same file and the chart refers to the source sheet, False means the copied chart's data source will not be changed. True means the copied chart's data source refers to the destination sheet.

```javascript
getReferToDestinationSheet() : boolean;
```


**Remarks**

The default value is false, it works as MS Excel.

### setReferToDestinationSheet(boolean) {#setReferToDestinationSheet-boolean-}

When copying the range in the same file and the chart refers to the source sheet, False means the copied chart's data source will not be changed. True means the copied chart's data source refers to the destination sheet.

```javascript
setReferToDestinationSheet(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

The default value is false, it works as MS Excel.


