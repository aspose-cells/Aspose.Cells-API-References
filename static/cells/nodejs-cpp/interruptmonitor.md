##InterruptMonitor
Represents all operator about the interrupt.
## InterruptMonitor class
Represents all operator about the interrupt.
```javascript
class InterruptMonitor;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Methods
| Method | Description |
| --- | --- |
| [interrupt()](#interrupt--)| Interrupt the current operator. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [isInterruptionRequested()](#isInterruptionRequested--)| Mark the monitor as requesting interruption |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### interrupt() {#interrupt--}
Interrupt the current operator.
```javascript
interrupt() : void;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### isInterruptionRequested() {#isInterruptionRequested--}
Mark the monitor as requesting interruption
```javascript
isInterruptionRequested() : boolean;
```
