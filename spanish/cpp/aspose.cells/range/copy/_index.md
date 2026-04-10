---
title: Aspose::Cells::Range::Copy method
linktitle: Copy
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Range::Copy method. Copying the range with paste special options in C++.'
type: docs
weight: 4600
url: /es/cpp/aspose.cells/range/copy/
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
//Instanciando un objeto Workbook
Workbook workbook;
// Obtener las primeras celdas de la hoja de cálculo.
Cells cells = workbook.GetWorksheets().Get(0).GetCells();
Range range1 = cells.CreateRange(u"A1:A5");
Range range2 = cells.CreateRange(u"A6:A10");
//Copiar el rango.
range1.Copy(range2);
//Guardar el archivo Excel
workbook.Save(u"book1.xlsm");

Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../vector/)
* Class [Range](../)
* Class [Range](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
