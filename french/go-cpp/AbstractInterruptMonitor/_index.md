---
title: "Classe AbstractInterruptMonitor"
linktitle: "AbstractInterruptMonitor"
second_title: "Référence API C++ d'Aspose.Cells pour Go"
description: "Classe AbstractInterruptMonitor. Encapsule l'objet qui représente abstractinterruptmonitor en Go."
type: docs
weight: 200
url: /fr/go-cpp/abstractinterruptmonitor/
---

## AbstractInterruptMonitor class

Surveille les demandes d'interruption dans toutes les opérations longues.

```go

type AbstractInterruptMonitor struct  {
	ptr unsafe.Pointer
}

```
## Constructeurs

| Méthode | Description |
| --- | --- |

## Méthodes

| Méthode | Description |
| --- | --- |
| [GetTerminateWithoutException](./getterminatewithoutexception/) | Lorsque la procédure est interrompue, qu'il faut terminer la procédure silencieusement ou lancer une Exception. La valeur par défaut est false, c'est‑à‑dire que lorsque IsInterruptionRequested est true, une CellsException avec le code ExceptionType.Interrupted sera lancée. |
