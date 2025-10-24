##Cells.ImportArrayList
Cells method. Imports an arraylist of data into a worksheet
## Cells.ImportArrayList method
Imports an arraylist of data into a worksheet.
```csharp
public void ImportArrayList(ArrayList arrayList, int firstRow, int firstColumn, bool isVertical)
```
| Parameter | Type | Description |
| --- | --- | --- |
| arrayList | ArrayList | Data arraylist. |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |
| isVertical | Boolean | Specifies to import data vertically or horizontally. |
### Examples
```csharp
using System;
using System.Collections;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodImportArrayListWithArrayListInt32Int32BooleanDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
ArrayList data = new ArrayList();
data.Add("Name");
data.Add("Age");
data.Add("City");
cells.ImportArrayList(data, 0, 0, false);
data.Clear();
data.Add("John");
data.Add(30);
data.Add("New York");
cells.ImportArrayList(data, 1, 0, false);
workbook.Save("ImportArrayListDemo.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
