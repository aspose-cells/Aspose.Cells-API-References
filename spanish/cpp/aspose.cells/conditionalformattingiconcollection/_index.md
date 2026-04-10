---
title: Aspose::Cells::ConditionalFormattingIconCollection class
linktitle: ConditionalFormattingIconCollection
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::ConditionalFormattingIconCollection class. Represents a collection of ConditionalFormattingIcon objects in C++.'
type: docs
weight: 3300
url: /es/cpp/aspose.cells/conditionalformattingiconcollection/
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
//Instanciando un objeto Workbook
Workbook workbook;

Worksheet sheet = workbook.GetWorksheets().Get(0);

//Obtener formato condicional
ConditionalFormattingCollection cformattings = sheet.GetConditionalFormattings();

//Agrega un formato condicional vacío
int index = cformattings.Add();

//Obtener formato condicional recién añadido
FormatConditionCollection fcs = cformattings.Get(index);

//Establece el rango del formato condicional.
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

//Establece condición
int idx = fcs.AddCondition(FormatConditionType::IconSet);

FormatCondition cond = fcs.Get(idx);

//Establece el tipo de condición
cond.GetIconSet().SetType(IconSetType::ArrowsGray3);

//Agregar condición de conjunto de íconos personalizada.
ConditionalFormattingIcon cfIcon = cond.GetIconSet().GetCfIcons().Get(0);

cfIcon.SetType(IconSetType::Arrows3);

cfIcon.SetIndex(0);

ConditionalFormattingIcon cfIcon1 = cond.GetIconSet().GetCfIcons().Get(1);

cfIcon1.SetType(IconSetType::ArrowsGray3);

cfIcon1.SetIndex(1);

ConditionalFormattingIcon cfIcon2 = cond.GetIconSet().GetCfIcons().Get(2);

cfIcon2.SetType(IconSetType::Boxes5);

cfIcon2.SetIndex(2);

//Guardando el archivo Excel
workbook.Save(u"output.xls");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
