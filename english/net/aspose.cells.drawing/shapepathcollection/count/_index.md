---
title: ShapePathCollection.Count
second_title: Aspose.Cells for .NET API Reference
description: ShapePathCollection property. Gets the count of paths
type: docs
url: /net/aspose.cells.drawing/shapepathcollection/count/
---
## ShapePathCollection.Count property

Gets the count of paths

```csharp
public int Count { get; }
```

### Examples

```csharp
// Called: Console.WriteLine("Number of paths in the ShapePathCollection: " + shapePaths.Count);
public static void ShapePathCollection_Property_Count()
        {



            // Instantiate a new Workbook
            Workbook workbook = new Workbook("ShapePathCollectionExample_original.xlsx");
            Worksheet worksheet = workbook.Worksheets[0];

            Shape customShape = worksheet.Shapes[0];
            
            // Access the ShapePathCollection of the arc shape
            ShapePathCollection shapePaths = customShape.Paths;

            if (shapePaths != null)
            {
                // Add a new path to the ShapePathCollection
                int pathIndex = shapePaths.Add();

                // Access the newly added ShapePath
                ShapePath newPath = shapePaths[pathIndex];

                // Display the count of paths in the ShapePathCollection
                Console.WriteLine("Number of paths in the ShapePathCollection: " + shapePaths.Count);
            }
            

            // Save the workbook
            workbook.Save("ShapePathCollectionExample.xlsx");
        }
```

### See Also

* class [ShapePathCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


