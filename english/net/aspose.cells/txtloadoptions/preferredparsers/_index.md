---
title: TxtLoadOptions.PreferredParsers
second_title: Aspose.Cells for .NET API Reference
description: TxtLoadOptions property. Gets and sets preferred value parsers for loading text file
type: docs
url: /net/aspose.cells/txtloadoptions/preferredparsers/
---
## TxtLoadOptions.PreferredParsers property

Gets and sets preferred value parsers for loading text file.

```csharp
public ICustomParser[] PreferredParsers { get; set; }
```

### Remarks

parsers[0] is the parser will be used for the first column in text template file, parsers[1] is the parser will be used for the second column, ...etc. The last one(parsers[parsers.length-1]) will be used for all other columns start from parsers.length-1. If one item is null, the corresponding column will be parsed by the default parser of Aspose.Cells.

### See Also

* interface [ICustomParser](../../icustomparser/)
* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


