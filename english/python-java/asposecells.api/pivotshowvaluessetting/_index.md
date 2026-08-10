---
title: "PivotShowValuesSetting Class"
linktitle: "PivotShowValuesSetting"
articleTitle: "PivotShowValuesSetting"
second_title: "Aspose.Cells for Python via Java"
description: "Represents the settings about showing values as when the ShowDataAs calculation is in use."
type: docs
weight: 4810
url: /python-java/asposecells.api/pivotshowvaluessetting/
---

## PivotShowValuesSetting class

Represents the settings about showing values as when the ShowDataAs calculation is in use.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [CalculationType](#calculationtype) | int | Represents how to show values of a data field in the pivot report. The value of the property is PivotFieldDataDisplayFor |
| [BaseFieldIndex](#basefieldindex) | int | Represents the base field for a ShowDataAs calculation when the ShowDataAs calculation is in use. |
| [BaseItemPositionType](#baseitempositiontype) | int | Represents type of the base pivot item in the base field when the ShowDataAs calculation is in use. Valid only for data  |
| [BaseItemIndex](#baseitemindex) | int | Represents the custom index of the pivot item in the base field when the ShowDataAs calculation is in use. Valid only fo |

### PivotShowValuesSetting.CalculationType property {#calculationtype}

Represents how to show values of a data field in the pivot report. The value of the property is PivotFieldDataDisplayFormat integer constant.

**Type:** int

### PivotShowValuesSetting.BaseFieldIndex property {#basefieldindex}

Represents the base field for a ShowDataAs calculation when the ShowDataAs calculation is in use.

**Type:** int

### PivotShowValuesSetting.BaseItemPositionType property {#baseitempositiontype}

Represents type of the base pivot item in the base field when the ShowDataAs calculation is in use. Valid only for data fields. Because PivotItemPosition.Custom is only for read,if you need to set PivotItemPosition.Custom, please set PivotField.BaseItemIndex attribute. The value of the property is PivotItemPositionType integer constant.

**Type:** int

### PivotShowValuesSetting.BaseItemIndex property {#baseitemindex}

Represents the custom index of the pivot item in the base field when the ShowDataAs calculation is in use. Valid only for data fields.

**Type:** int
