---
title: "Método GetRefreshOnChange"
linktitle: "GetRefreshOnChange"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Método GetRefreshOnChange. Encapsula la función que representa getrefreshonchange en Go."
type: docs
weight: 200
url: /es/go-cpp/connectionparameter/getrefreshonchange/
---

## GetRefreshOnChange function

Flag indicating whether the query should automatically refresh when the contents of acell that provides the parameter value changes. If true, then external data is refreshedusing the new parameter value every time there's a change. If false, then external datais only refreshed when requested by the user, or some other event triggers refresh (e.g., workbook opened).

```go

func (instance *ConnectionParameter) GetRefreshOnChange()  (bool,  error) 

```

## Observaciones


## Ver también

* Class [ConnectionParameter](../)
* Library [Aspose.Cells for Go](../../)
