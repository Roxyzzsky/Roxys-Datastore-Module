---
hide:
  - footer
---

# Datastoreobj

This objects gets returned by the {==Datastore.new()==} constructor and is used to manage a Datastore in its entirety along with the data within it.

## General Structure

The general structure of a datastoreObj looks like the following example:
```
<datastoreName> = {
  _datastore = <RBXDatastore>,
  _template = <datastoreTemplate>,
  registeredClients = <array -> Player>,
  events = <array -> BindableEvent>
  <datastoreObj methods>
}
```

??? info "Variable explanation"
    **_datastore** - The Datastore instance normally provided by :GetDataStore()
    <br>
    **_template** - A template for the user's data that will be used if :GetAsync() returns nil
    <br>
    **registeredClients** - An array containing all players whose data has been loaded (along with said data)
    <br>
    **events** - An array containing various BindableEvents that will fire in certain scenarios (see [Events](#events))
    <br>
    **datastoreObj methods** - All methods provided to a datastoreObj (see [Methods](#methods))

## Methods

## Events