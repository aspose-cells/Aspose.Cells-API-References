---
title: "Classe ProtectedRange"
linktitle: "ProtectedRange"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe ProtectedRange. Incapsula l'oggetto che rappresenta protectedrange in Go."
type: docs
weight: 200
url: /it/go-cpp/protectedrange/
---

## ProtectedRange class

Un intervallo specificato che può essere modificato quando la protezione del foglio è ATTIVA.

```go

type ProtectedRange struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetName](./getname/) | Restituisce il titolo del Range. Viene usato come descrittore, non come definizione di intervallo nominato. |
| [SetName](./setname/) | Restituisce il titolo del Range. Viene usato come descrittore, non come definizione di intervallo nominato. |
| [GetCellArea](./getcellarea/) | Restituisce l'oggetto CellArea che rappresenta l'area di celle da proteggere. |
| [GetAreas](./getareas/) | Restituisce tutte le aree riferite. |
| [AddArea](./addarea/) | Aggiunge un'area riferita a questo. |
| [IsProtectedWithPassword](./isprotectedwithpassword/) | Indica se il foglio di lavoro è protetto da password. |
| [GetPassword](./getpassword/) | Rappresenta la password per proteggere l'intervallo. |
| [SetPassword](./setpassword/) | Rappresenta la password per proteggere l'intervallo. |
| [GetSecurityDescriptor](./getsecuritydescriptor/) | Il descrittore di sicurezza definisce gli account utente che possono modificare questo intervallo senza fornire una password per accedere all'intervallo. |
| [SetSecurityDescriptor](./setsecuritydescriptor/) | Il descrittore di sicurezza definisce gli account utente che possono modificare questo intervallo senza fornire una password per accedere all'intervallo. |
