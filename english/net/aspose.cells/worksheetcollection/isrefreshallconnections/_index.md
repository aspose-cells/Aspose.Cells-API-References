---
title: WorksheetCollection.IsRefreshAllConnections
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection property. Indicates whether refresh all connections on opening file in MS Excel
type: docs
url: /net/aspose.cells/worksheetcollection/isrefreshallconnections/
---
## WorksheetCollection.IsRefreshAllConnections property

Indicates whether refresh all connections on opening file in MS Excel.

```csharp
public bool IsRefreshAllConnections { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(expected.IsRefreshAllConnections,result.IsRefreshAllConnections, info + ".IsRefreshAllConnections");
private static void WorksheetCollection_Property_IsRefreshAllConnections(WorksheetCollection expected, WorksheetCollection result, string info)
        {
            AssertHelper.AreEqual(expected.ActiveSheetIndex, result.ActiveSheetIndex, info + ".ActiveSheetIndex");
            // AssertHelper.AreEqual(arrsheetSrc.EnableHTTPCompression, arrsheetDest.EnableHTTPCompression, info + ".EnableHTTPCompression");
          
           AssertHelper.AreEqual(expected.IsRefreshAllConnections,result.IsRefreshAllConnections, info + ".IsRefreshAllConnections");
        }
```

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


