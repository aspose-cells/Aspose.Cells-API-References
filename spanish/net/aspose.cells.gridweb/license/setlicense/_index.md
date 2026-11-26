---
title: "License.SetLicense"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método License. Licencia el componente"
type: docs
url: /es/net/aspose.cells.gridweb/license/setlicense/
---
## SetLicense(Stream) {#setlicense}

Licencia el componente.

```csharp
public void SetLicense(Stream stream)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | Stream | Un flujo que contiene la licencia. |

### Observaciones

Utilice este método para cargar una licencia desde un flujo.

### Ejemplos

```csharp
[C#]

License license = new License();
license.SetLicense(myStream);


[Visual Basic]

Dim license as License = new License
license.SetLicense(myStream)
```

### Ver también

* class [License](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## SetLicense(string) {#setlicense_1}

Licencia el componente.

```csharp
public void SetLicense(string licenseName)
```

### Observaciones

Intenta encontrar la licencia en las siguientes ubicaciones:

1. Ruta explícita.

2. La carpeta que contiene el ensamblado del componente Aspose.

3. La carpeta que contiene el ensamblado que llama el cliente.

4. La carpeta que contiene el ensamblado de entrada (inicio).

5. Un recurso incrustado en el ensamblado que llama el cliente.

**Note:**On the .NET Compact Framework, tries to find the license only in these locations:

1. Ruta explícita.

2. Un recurso incrustado en el ensamblado que llama el cliente.

### Ejemplos

En este ejemplo, se intentará encontrar un archivo de licencia llamado MyLicense.lic en la carpeta que contiene el componente, en la carpeta que contiene el ensamblado que llama, en la carpeta del ensamblado de entrada y luego en los recursos incrustados del ensamblado que llama.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As License = New License
license.SetLicense("MyLicense.lic")
```

Puede ser un nombre de archivo completo o corto o el nombre de un recurso incrustado. Use una cadena vacía para cambiar al modo de evaluación.

### Ver también

* class [License](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


