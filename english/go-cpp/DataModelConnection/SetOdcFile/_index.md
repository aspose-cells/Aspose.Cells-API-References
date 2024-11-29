---
title: SetOdcFile Method 
linktitle: SetOdcFile
second_title: Aspose.Cells for Go API Reference
description: 'SetOdcFile method. Encapsulates the function that represents setodcfile in Go.'
type: docs
weight: 200
url: /go/datamodelconnection/setodcfile/
---

## SetOdcFile function

Specifies the full path to external connection file from which this connection wascreated. If a connection fails during an attempt to refresh data, and reconnectionMethod=1,then the spreadsheet application will try again using information from the external connection fileinstead of the connection object embedded within the workbook.

```go

func (instance *DataModelConnection) SetOdcFile(value string)  error

```

## Remarks


## See Also

* Class [DataModelConnection](../)
* Namespace [Aspose.Cells.ExternalConnections](../../)
* Library [Aspose.Cells for Go](../../../)
