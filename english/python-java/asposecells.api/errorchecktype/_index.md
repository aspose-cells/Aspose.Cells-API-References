---
title: "ErrorCheckType Enum"
linktitle: "ErrorCheckType"
articleTitle: "ErrorCheckType"
second_title: "Aspose.Cells for Python via Java"
description: "Utility class containing constants."
type: docs
weight: 2140
url: /python-java/asposecells.api/errorchecktype/
---

## ErrorCheckType enumeration

Utility class containing constants. Represents all error check type.

## Values

| Name | Description |
| --- | --- |
| EVALUATION_ERROR | Ignore errors when cells contain formulas that result in an error. |
| CALC | NOTE: This member is now obsolete. Instead, please use ErrorCheckType.EvaluationError enum. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced. |
| EMPTY_CELL_REF | Ignore errors when formulas refer to empty cells. |
| NUMBER_STORED_AS_TEXT | Ignore errors when numbers are formatted as text or are preceded by an apostrophe |
| TEXT_NUMBER | Ignore errors when numbers are formatted as text or are preceded by an apostrophe NOTE: This member is now obsolete. Instead, please use ErrorCheckType.NumberStoredAsText enum. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced. |
| INCONSIST_RANGE | Ignore errors when formulas omit certain cells in a region. |
| INCONSIST_FORMULA | Ignore errors when a formula in a region of your worksheet differs from other formulas in the same region. |
| TWO_DIGIT_TEXT_YEAR | Ignore errors when formulas contain text formatted cells with years represented as 2 digits. |
| TEXT_DATE | Ignore errors when formulas contain text formatted cells with years represented as 2 digits. NOTE: This member is now obsolete. Instead, please use ErrorCheckType.TwoDigitTextYear enum. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced. |
| UNLOCKED_FORMULA | Ignore errors when unlocked cells contain formulas. |
| UNPROCTED_FORMULA | Ignore errors when unlocked cells contain formulas. NOTE: This member is now obsolete. Instead, please use ErrorCheckType.UnproctedFormula enum. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced. |
| TABLE_DATA_VALIDATION | Ignore errors when a cell's value in a Table does not comply with the Data Validation rules specified. |
| VALIDATION | Ignore errors when a cell's value in a Table does not comply with the Data Validation rules specified. NOTE: This member is now obsolete. Instead, please use ErrorCheckType.TableDataValidation enum. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced. |
| CALCULATED_COLUMN | Ignore errors when cells contain a value different from a calculated column formula. |
