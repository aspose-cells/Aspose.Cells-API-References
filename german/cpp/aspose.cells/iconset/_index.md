---
title: Aspose::Cells::IconSet class
linktitle: IconSet
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::IconSet class. Describe the IconSet conditional formatting rule. This conditional formatting rule applies icons to cells according to their values in C++.'
type: docs
weight: 8700
url: /de/cpp/aspose.cells/iconset/
---
## IconSet class


Describe the [IconSet](./) conditional formatting rule. This conditional formatting rule applies icons to cells according to their values.

```cpp
class IconSet
```

## Methods

| Method | Description |
| --- | --- |
| [GetCfIcons()](./getcficons/) | Get the[ConditionalFormattingIcon](../conditionalformattingicon/) from the collection. |
| [GetCfvos()](./getcfvos/) | Get the CFValueObjects instance. |
| [GetReverse()](./getreverse/) | Get or set the flag indicating whether to reverses the default order of the icons in this icon set. Default value is false. |
| [GetShowValue()](./getshowvalue/) | Get or set the flag indicating whether to show the values of the cells on which this icon set is applied. Default value is true. |
| [GetType()](./gettype/) | Get or Set the icon set type to display. Setting the type will auto check if the current Cfvos's count is accord with the new type. If not accord, old Cfvos will be cleaned and default Cfvos will be added. |
| [IconSet(IconSet_Impl* impl)](./iconset/) | Constructs from an implementation object. |
| [IconSet(const IconSet\& src)](./iconset/) | Copy constructor. |
| [IsCustom()](./iscustom/) | Indicates whether the icon set is custom. Default value is false. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const IconSet\& src)](./operator_asm/) | operator= |
| [SetReverse(bool value)](./setreverse/) | Get or set the flag indicating whether to reverses the default order of the icons in this icon set. Default value is false. |
| [SetShowValue(bool value)](./setshowvalue/) | Get or set the flag indicating whether to show the values of the cells on which this icon set is applied. Default value is true. |
| [SetType(IconSetType value)](./settype/) | Get or Set the icon set type to display. Setting the type will auto check if the current Cfvos's count is accord with the new type. If not accord, old Cfvos will be cleaned and default Cfvos will be added. |
| [~IconSet()](./~iconset/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
//Instanziieren eines Workbook-Objekts
Workbook workbook;

Worksheet sheet = workbook.GetWorksheets().Get(0);

//Fügt eine leere bedingte Formatierung hinzu
int index = sheet.GetConditionalFormattings().Add();

FormatConditionCollection fcs = sheet.GetConditionalFormattings().Get(index);

//Legt den Bereich der bedingten Formatierung fest.
CellArea ca;
ca.StartRow = 0;
ca.EndRow = 2;
ca.StartColumn = 0;
ca.EndColumn = 0;

fcs.AddArea(ca);

//Fügt Bedingung hinzu.
int idx = fcs.AddCondition(FormatConditionType::IconSet);

fcs.AddArea(ca);

FormatCondition cond = fcs.Get(idx);

//Icon-Set abrufen
IconSet iconSet = cond.GetIconSet();

//Icon-Typ festlegen
iconSet.SetType(IconSetType::Arrows3);

//Zellwerte einfügen
Cell cell1 = sheet.GetCells().Get(u"A1");
cell1.PutValue(10);

Cell cell2 = sheet.GetCells().Get(u"A2");
cell2.PutValue(120);

Cell cell3 = sheet.GetCells().Get(u"A3");
cell3.PutValue(260);

//Speichern der Excel-Datei
workbook.Save(u"book1.xlsx");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
