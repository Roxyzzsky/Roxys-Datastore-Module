---
hide:
  - footer
---

# Introduction

Heyo! Welcome to the documentation of this module. Feel free to look around and explore the API, I tried keeping it organized.
<br>
<br>
**Please note that this documentation is heavily WIP and will change as the module gets edited**

## Constructors

**new**
```lua
local datastore = Datastore.new()
```
Returns [datastoreObj](datastoreobjects.md).
---

## Methods

**safeTry**
<span class="badge badge-internal">Internal</span>
```lua
Datastore._safeTry(function, configuration)
```
Used to pcall a function with provided configuration. Mainly used within getAsync and SetAsync.

!!! note "Please note"
    Internal methods are not intented to be used by in-game scripts.
    Their purpose is to be used by the Methods within the Datastore module in order to prevent errors during runtime.

**getStore**
```lua
local datastore = Datastore.getStore(name)
```
Returns a [datastoreObj](datastoreobjects.md) that matches the specified name.

**getStores**
```lua
local datastores = Datastore.getStores()
```
Returns an array of all available [datastoreObjs](datastoreobjects.md). The individual datastoreobjects will be indexed via their name they were initialized with.