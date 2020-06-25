# VIP template for Generamba with SwiftUI

Our own impletation VIP in SwiftUI

1) Module has model with state, called *Your_Module_name*ViewModel.swift
2) View and Presenter has reference to this ViewModule. Every change in ViewModule call refresh View that has this ViewModel.
3) For  navigation you can use "Router" property in *Your_Module_name*View.swift

## How to use
You need some BaseClasses
1. DIResolver

### DIResolver
```swift
class DIResolver {

    init() { }

}
```
Then just use this :)

Don't use *update(model..)* func for update your UI! Use viewModule only!
