---
title: "License.SetLicense"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo License. Concede la licenza al componente"
type: docs
url: /it/net/aspose.cells/license/setlicense/
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

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LicenseMethodSetLicenseWithStringDemo
    {
        public static void Run()
        {
            License license = new License();
            license.SetLicense("MyLicense.lic");
            
            Console.WriteLine("License set successfully.");
        }
    }
}
```

### Vedi anche

* class [License](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

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
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


