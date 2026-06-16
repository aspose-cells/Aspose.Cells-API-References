---
title: Aspose::Cells::ConditionalFormattingIconCollection class
linktitle: ConditionalFormattingIconCollection
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::ConditionalFormattingIconCollection class. Represents a collection of ConditionalFormattingIcon objects in C++.'
type: docs
weight: 3300
url: /fr/cpp/aspose.cells/conditionalformattingiconcollection/
---
## ConditionalFormattingIconCollection class


Represents a collection of [ConditionalFormattingIcon](../conditionalformattingicon/) objects.

```cpp
class ConditionalFormattingIconCollection
```

## Methods

| Method | Description |
| --- | --- |
| [Add(IconSetType type, int32_t index)](./add/) | Adds [ConditionalFormattingIcon](../conditionalformattingicon/) object. |
| [Add(const ConditionalFormattingIcon\& cficon)](./add/) |  **(Deprecated)** Adds [ConditionalFormattingIcon](../conditionalformattingicon/) object. |
| [ConditionalFormattingIconCollection(ConditionalFormattingIconCollection_Impl* impl)](./conditionalformattingiconcollection/) | Constructs from an implementation object. |
| [ConditionalFormattingIconCollection(const ConditionalFormattingIconCollection\& src)](./conditionalformattingiconcollection/) | Copy constructor. |
| [Get(int32_t index)](./get/) | Gets the [ConditionalFormattingIcon](../conditionalformattingicon/) element at the specified index. |
| [GetCount()](./getcount/) |  |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ConditionalFormattingIconCollection\& src)](./operator_asm/) | operator= |
| [~ConditionalFormattingIconCollection()](./~conditionalformattingiconcollection/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
//Instanciation d'un objet Workbook
Workbook workbook;

Worksheet sheet = workbook.GetWorksheets().Get(0);

//Obtenir la mise en forme conditionnelle
ConditionalFormattingCollection cformattings = sheet.GetConditionalFormattings();

//Ajoute une mise en forme conditionnelle vide
int index = cformattings.Add();

//Obtenir la mise en forme conditionnelle nouvellement ajoutée
FormatConditionCollection fcs = cformattings.Get(index);

//Définit la plage de mise en forme conditionnelle.
CellArea ca;
ca.StartRow = 0;
ca.EndRow = 0;
ca.StartColumn = 0;
ca.EndColumn = 0;
fcs.AddArea(ca);

ca = CellArea();
ca.StartRow = 1;
ca.EndRow = 1;
ca.StartColumn = 1;
ca.EndColumn = 1;
fcs.AddArea(ca);

//Sets condition
int idx = fcs.AddCondition(FormatConditionType::IconSet);

FormatCondition cond = fcs.Get(idx);

//Sets condition's type
cond.GetIconSet().SetType(IconSetType::ArrowsGray3);

//Add custom iconset condition.
ConditionalFormattingIcon cfIcon = cond.GetIconSet().GetCfIcons().Get(0);

cfIcon.SetType(IconSetType::Arrows3);

cfIcon.SetIndex(0);

ConditionalFormattingIcon cfIcon1 = cond.GetIconSet().GetCfIcons().Get(1);

cfIcon1.SetType(IconSetType::ArrowsGray3);

cfIcon1.SetIndex(1);

ConditionalFormattingIcon cfIcon2 = cond.GetIconSet().GetCfIcons().Get(2);

cfIcon2.SetType(IconSetType::Boxes5);

cfIcon2.SetIndex(2);

//Enregistrement du fichier Excel
workbook.Save(u"output.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
