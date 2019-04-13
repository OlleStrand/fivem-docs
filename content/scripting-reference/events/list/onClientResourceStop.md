---
title: onClientResourceStop
weight: 546
---

Called when a resource stops.

Parameters
----------

```
string resourceName
```

- resourceName: The name of the resource that stopped.

Examples
--------
This example prints the name of a resource that was just stopped.

##### Lua Example:
```lua
AddEventHandler('onClientResourceStop', function (resourceName)
  print('The resource ' .. resourceName .. ' has been stopped on the client.')
end)
```

##### C\# Example:
```csharp
// In class constructor
EventHandlers["onClientResourceStop"] += new Action<string>(OnClientResourceStop);

// Delegate method
private void OnClientResourceStop(string resourceName)
{
    Debug.WriteLine($"The resource {resourceName} has been stopped on the client.");
}
```
