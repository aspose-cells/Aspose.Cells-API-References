---
title: "AutoFitterOptions Class"
linktitle: "AutoFitterOptions"
articleTitle: "AutoFitterOptions"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents all auto fitter options."
type: docs
weight: 200
url: /php/aspose.cells/autofitteroptions/
---

## AutoFitterOptions class

Represents all auto fitter options.

## Constructors

| Name | Description |
| --- | --- |
| [AutoFitterOptions](#constructor) |  |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [DefaultEditLanguage](#defaulteditlanguage) | Number | Gets or sets default edit language. The value of the property is DefaultEditLanguage integer constant. It may display/re |
| [AutoFitMergedCells](#autofitmergedcells) | boolean | Indicates whether auto fit row height when the cells is merged in a row. The default value is false. NOTE: This member i |
| [AutoFitMergedCellsType](#autofitmergedcellstype) | Number | Gets and set the type of auto fitting row height of merged cells. The value of the property is AutoFitMergedCellsType in |
| [OnlyAuto](#onlyauto) | boolean | Indicates whether only fit the rows which height are not customed. |
| [IgnoreHidden](#ignorehidden) | boolean | Ignores the hidden rows/columns. |
| [MaxRowHeight](#maxrowheight) | Number | Gets and sets the max row height(in unit of Point) when autofitting rows. |
| [AutoFitWrappedTextType](#autofitwrappedtexttype) | Number | Gets and sets the type of auto fitting wrapped text. The value of the property is AutoFitWrappedTextType integer constan |
| [FormatStrategy](#formatstrategy) | Number | Gets and sets the formatted strategy. The value of the property is CellValueFormatStrategy integer constant. The default |
| [ForRendering](#forrendering) | boolean | Indicates whether fit for rendering purpose. |

### AutoFitterOptions() {#constructor}

### AutoFitterOptions.DefaultEditLanguage property {#defaulteditlanguage}

Gets or sets default edit language. The value of the property is DefaultEditLanguage integer constant. It may display/render different layouts for text paragraph when different edit languages is set. Default is DefaultEditLanguage.AUTO .

**Type:** Number

### AutoFitterOptions.AutoFitMergedCells property {#autofitmergedcells}

Indicates whether auto fit row height when the cells is merged in a row. The default value is false. NOTE: This member is now obsolete. Instead, please use AutoFitterOptions.AutoFitMergedCellsType property, instead. This property will be removed 12 months later since December 2018. Aspose apologizes for any inconvenience you may have experienced.

**Type:** boolean

### AutoFitterOptions.AutoFitMergedCellsType property {#autofitmergedcellstype}

Gets and set the type of auto fitting row height of merged cells. The value of the property is AutoFitMergedCellsType integer constant. Excel defaults to ignore merged cells when fitting the row height, so Aspose.Cells works as MS Excel default. Please set this type to change the way of auto fitting row height of merged cells.

**Type:** Number

### AutoFitterOptions.OnlyAuto property {#onlyauto}

Indicates whether only fit the rows which height are not customed.

**Type:** boolean

### AutoFitterOptions.IgnoreHidden property {#ignorehidden}

Ignores the hidden rows/columns.

**Type:** boolean

### AutoFitterOptions.MaxRowHeight property {#maxrowheight}

Gets and sets the max row height(in unit of Point) when autofitting rows.

**Type:** Number

### AutoFitterOptions.AutoFitWrappedTextType property {#autofitwrappedtexttype}

Gets and sets the type of auto fitting wrapped text. The value of the property is AutoFitWrappedTextType integer constant.

**Type:** Number

### AutoFitterOptions.FormatStrategy property {#formatstrategy}

Gets and sets the formatted strategy. The value of the property is CellValueFormatStrategy integer constant. The default value is CellStyle for performance.

**Type:** Number

### AutoFitterOptions.ForRendering property {#forrendering}

Indicates whether fit for rendering purpose.

**Type:** boolean
