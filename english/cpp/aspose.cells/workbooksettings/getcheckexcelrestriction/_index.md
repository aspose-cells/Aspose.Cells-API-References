﻿---
title: Aspose::Cells::WorkbookSettings::GetCheckExcelRestriction method
linktitle: GetCheckExcelRestriction
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::WorkbookSettings::GetCheckExcelRestriction method. Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell''s value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file in C++.'
type: docs
weight: 9400
url: /cpp/aspose.cells/workbooksettings/getcheckexcelrestriction/
---
## WorkbookSettings::GetCheckExcelRestriction method


Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file.

```cpp
bool Aspose::Cells::WorkbookSettings::GetCheckExcelRestriction()
```

## See Also

* Class [Vector](../../vector/)
* Class [WorkbookSettings](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
