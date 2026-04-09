---
title: Aspose::Cells::Range::Copy method
linktitle: Copy
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Range::Copy method. Copying the range with paste special options in C++.'
type: docs
weight: 4600
url: /de/cpp/aspose.cells/range/copy/
---
## Range::Copy(const Range\&, const PasteOptions\&) method


Copying the range with paste special options.

```cpp
void Aspose::Cells::Range::Copy(const Range &range, const PasteOptions &options)
```


| Parameter | Type | Description |
| --- | --- | --- |
| range | const Range\& | The source range. |
| options | const PasteOptions\& | The paste special options. |

## See Also

* Class [Vector](../../vector/)
* Class [Range](../)
* Class [PasteOptions](../../pasteoptions/)
* Class [Range](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Range::Copy(const Range\&) method


Copies data (including formulas), formatting, drawing objects etc. from a source range.

```cpp
void Aspose::Cells::Range::Copy(const Range &range)
```


| Parameter | Type | Description |
| --- | --- | --- |
| range | const Range\& | Source [Range](../) object. |


## Examples


```cpp
Aspose::Cells::Startup();
//Instanziieren eines Workbook-Objekts
Workbook workbook;
// Die Zellen des ersten Arbeitsblatts abrufen.
Cells cells = workbook.GetWorksheets().Get(0).GetCells();
Range range1 = cells.CreateRange(u"A1:A5");
Range range2 = cells.CreateRange(u"A6:A10");
//Kopiere den Bereich.
range1.Copy(range2);
//Excel-Datei speichern
workbook.Save(u"book1.xlsm");

Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../vector/)
* Class [Range](../)
* Class [Range](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
