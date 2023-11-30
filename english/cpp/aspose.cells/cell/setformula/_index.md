---
title: Aspose::Cells::Cell::SetFormula method
linktitle: SetFormula
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Cell::SetFormula method. Gets or sets a formula of the Cell in C++.'
type: docs
weight: 3300
url: /cpp/aspose.cells/cell/setformula/
---
## Cell::SetFormula(const U16String\&) method


Gets or sets a formula of the [Cell](../).

```cpp
void Aspose::Cells::Cell::SetFormula(const U16String &value)
```

## Remarks


A formula string always begins with an equal sign (=). And please always use comma(,) as parameters delimiter, such as "=SUM(A1, E1, H2)". 

## Examples


```cpp
Aspose::Cells::Startup();
Workbook excel;
Cells cells = excel.GetWorksheets().Get(0).GetCells();
U16String f = u"=SUM(B2:B5, E1) + sheet1!A1";
cells.Get(u"B6").SetFormula(f);
Aspose::Cells::Cleanup();
```

## See Also

* Class [U16String](../../u16string/)
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cell::SetFormula(const char16_t*) method


Gets or sets a formula of the [Cell](../).

```cpp
void Aspose::Cells::Cell::SetFormula(const char16_t *value)
```

## Remarks


A formula string always begins with an equal sign (=). And please always use comma(,) as parameters delimiter, such as "=SUM(A1, E1, H2)". 

## Examples


```cpp
Aspose::Cells::Startup();
Workbook excel;
Cells cells = excel.GetWorksheets().Get(0).GetCells();
cells.Get(u"B6").SetFormula(u"=SUM(B2:B5, E1) + sheet1!A1");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
