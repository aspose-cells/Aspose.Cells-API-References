---
title: "License.SetLicense"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo License. Concede la licenza al componente"
type: docs
url: /it/net/aspose.cells.griddesktop/license/setlicense/
---
## SetLicense(Stream) {#setlicense}

Licenzia il componente.

```csharp
public void SetLicense(Stream stream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | Uno stream che contiene la licenza. |

### Osservazioni

Usa questo metodo per caricare una licenza da uno stream.

### Esempi

```csharp
[C#]

License license = new License();
license.SetLicense(myStream);


[Visual Basic]

Dim license as License = new License
license.SetLicense(myStream)
```

### Vedi anche

* class [License](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## SetLicense(string) {#setlicense_1}

Licenzia il componente.

```csharp
public void SetLicense(string licenseName)
```

### Osservazioni

Cerca di trovare la licenza nei seguenti percorsi:

1. Percorso esplicito.

2. La cartella che contiene l'assembly del componente Aspose.

3. La cartella che contiene l'assembly chiamante del client.

4. La cartella che contiene l'assembly di ingresso (avvio).

5. Una risorsa incorporata nell'assembly chiamante del client.

**Note:**On the .NET Compact Framework, tries to find the license only in these locations:

1. Percorso esplicito.

2. Una risorsa incorporata nell'assembly chiamante del client.

### Esempi

In questo esempio, si cercherà di trovare un file di licenza denominato MyLicense.lic nella cartella che contiene il componente, nella cartella che contiene l'assembly chiamante, nella cartella dell'assembly di ingresso e poi nelle risorse incorporate dell'assembly chiamante.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As License = New License
license.SetLicense("MyLicense.lic")
```

Può essere un nome file completo o breve o il nome di una risorsa incorporata. Usa una stringa vuota per passare alla modalità di valutazione.

### Vedi anche

* class [License](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


