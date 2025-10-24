##PictureCollection.RemoveAt
PictureCollection method. Remove shapes at the specific index
## PictureCollection.RemoveAt method
Remove shapes at the specific index
```csharp
public void RemoveAt(int index)
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PictureCollectionMethodRemoveAtWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some pictures to the worksheet
int index1 = worksheet.Pictures.Add(1, 1, "image1.png");
int index2 = worksheet.Pictures.Add(5, 1, "image2.png");
int index3 = worksheet.Pictures.Add(10, 1, "image3.png");
Console.WriteLine("Number of pictures before removal: " + worksheet.Pictures.Count);
// Remove the picture at specified index
worksheet.Pictures.RemoveAt(index2);
Console.WriteLine("Number of pictures after removal: " + worksheet.Pictures.Count);
}
}
}
```
### See Also
* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
