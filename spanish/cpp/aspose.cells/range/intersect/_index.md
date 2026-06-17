---
title: Aspose::Cells::Range::Intersect method
linktitle: Intersect
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Range::Intersect method. Returns a Range object that represents the rectangular intersection of two ranges in C++.'
type: docs
weight: 1200
url: /es/cpp/aspose.cells/range/intersect/
---
## Range::Intersect method


Returns a [Range](../) object that represents the rectangular intersection of two ranges.

```cpp
Range Aspose::Cells::Range::Intersect(const Range &range)
```


| Parameter | Type | Description |
| --- | --- | --- |
| range | const Range\& | The intersecting range. |

## ReturnValue

Returns a [Range](../) object
## Remarks



If the two ranges are not intersected, returns null.

## Examples


```cpp
Aspose::Cells::Startup();
//Instanciando un objeto Workbook
Workbook workbook;
// Obtener las primeras celdas de la hoja de cálculo.
Cells cells = workbook.GetWorksheets().Get(0).GetCells();
Range range1 = cells.CreateRange(u"A1:A5");
Range range2 = cells.CreateRange(u"A3:A10");
//Obtener el rango intersectado de los dos rangos.
Range intersectRange = range1.Intersect(range2);
//Guardar el archivo Excel
workbook.Save(u"book1.xlsm");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Range](../)
* Class [Vector](../../vector/)
* Class [Range](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
