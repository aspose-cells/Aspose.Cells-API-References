---
title: Equals
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Determina se questa istanza ha lo stesso valore di unaltra specificataLineFormataspose.cells.drawing/lineformat oggetto.
type: docs
weight: 120
url: /it/net/aspose.cells.drawing/lineformat/equals/
---
## LineFormat.Equals method

Determina se questa istanza ha lo stesso valore di un'altra specificata[`LineFormat`](../../lineformat) oggetto.

```csharp
public override bool Equals(object obj)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | Object | Il[`LineFormat`](../../lineformat) oggetto da confrontare con questa istanza. |

### Valore di ritorno

true se il valore del parametro obj è uguale al valore di questa istanza; altrimenti falso. Se obj è null, questo metodo restituisce false.

### Esempi

```csharp

[C#]
//Devi assicurarti che il valore dell'indice in questa riga di codice esista
LineFormat obj = workbook.Worksheets[0].Shapes[0].Line;
if (lineFmt.Equals(obj))
{
    //Fai quello che vuoi
}

```

### Guarda anche

* class [LineFormat](../../lineformat)
* spazio dei nomi [Aspose.Cells.Drawing](../../lineformat)
* assemblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
