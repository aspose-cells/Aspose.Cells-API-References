---
title: GetSeverCommand Method 
linktitle: GetSeverCommand
second_title: Aspose.Cells for Go API Reference
description: 'GetSeverCommand method. Encapsulates the function that represents getsevercommand in Go.'
type: docs
weight: 200
url: /go/aspose.cells.externalconnections/dbconnection/getsevercommand/
---

## GetSeverCommand function

Specifies a second command text string that is persisted when PivotTable server-basedpage fields are in use.For ODBC connections, serverCommand is usually a broader query than command (noWHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand),parameter UI can be populated and parameterized queries can be constructed

```go

func (instance *DBConnection) GetSeverCommand()  (string,  error) 

```

## Remarks


## See Also

* Class [DBConnection](../)
* Namespace [Aspose.Cells.ExternalConnections](../../)
* Library [Aspose.Cells for Go](../../../)
