---
title: Aspose::Cells::Pivot::PivotFieldGroupSettings class
linktitle: PivotFieldGroupSettings
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Pivot::PivotFieldGroupSettings class. Represents the group setting of pivot field in C++.'
type: docs
weight: 1700
url: /sv/cpp/aspose.cells.pivot/pivotfieldgroupsettings/
---
## PivotFieldGroupSettings class


Represents the group setting of pivot field.

```cpp
class PivotFieldGroupSettings
```

## Methods

| Method | Description |
| --- | --- |
| [GetType()](./gettype/) | Gets the group type of pivot field. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const PivotFieldGroupSettings\& src)](./operator_asm/) | operator= |
| [PivotFieldGroupSettings()](./pivotfieldgroupsettings/) | Default constructor. |
| [PivotFieldGroupSettings(PivotFieldGroupSettings_Impl* impl)](./pivotfieldgroupsettings/) | Constructs from an implementation object. |
| [PivotFieldGroupSettings(const PivotFieldGroupSettings\& src)](./pivotfieldgroupsettings/) | Copy constructor. |
| [~PivotFieldGroupSettings()](./~pivotfieldgroupsettings/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
// Läs in exempelarbetsboken
Workbook wb(u"sampleGroupPivotFieldsInPivotTable.xlsx");
// Åtkomst till det andra kalkylbladet och dess pivottabell
PivotTable pt = wb.GetWorksheets().Get(1).GetPivotTables().Get(0);
// FieldTwo är ett datafält: flytta det till radområdet först,
// eftersom endast rad-/kolumnfält kan grupperas
pt.AddFieldToArea(PivotFieldType::Row, u"FieldTwo");
pt.CalculateData();
// Gruppera det numeriska fältet i intervallen 0-1, 2-3, 4-5
PivotFieldGroupOptions options;
options.SetStartNumber(0);
options.SetEndNumber(5);
options.SetInterval(2);
pt.GetRowFields().Get(1).Group(options);
// Beräkna pivottabellsdata och spara utdatafilen
pt.CalculateData();
wb.Save(u"outputNumberGroupPivotField.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells::Pivot](../)
* Library [Aspose.Cells for C++](../../)
