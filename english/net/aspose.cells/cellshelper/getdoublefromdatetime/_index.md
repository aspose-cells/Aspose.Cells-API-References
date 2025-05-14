---
title: CellsHelper.GetDoubleFromDateTime
second_title: Aspose.Cells for .NET API Reference
description: CellsHelper method. Convert the date time to double value
type: docs
url: /net/aspose.cells/cellshelper/getdoublefromdatetime/
---
## CellsHelper.GetDoubleFromDateTime method

Convert the date time to double value.

```csharp
public static double GetDoubleFromDateTime(DateTime dateTime, bool date1904)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dateTime | DateTime | The date time. |
| date1904 | Boolean | Date 1904 system. |

### Examples

```csharp
// Called: Assert.AreEqual((int)cells["A1"].DoubleValue,(int)CellsHelper.GetDoubleFromDateTime(DateTime.Now,false));
public void CellsHelper_Method_GetDoubleFromDateTime()
{
  Workbook workbook = new Workbook();
  Cells cells = workbook.Worksheets[0].Cells;
  cells[0, 0].Formula = "=NOW(  )";
  workbook.CalculateFormula();
    Assert.AreEqual((int)cells["A1"].DoubleValue,(int)CellsHelper.GetDoubleFromDateTime(DateTime.Now,false));
 // Console.WriteLine(cells[0, 0].DateTimeValue);
}
```

### See Also

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


