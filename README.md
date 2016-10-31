![](https://cdn-images-1.medium.com/max/2000/1*FIswW9fZgcLsflR9ok2w6w.jpeg)

# Swift: UserDefaults Protocol
## Swift eye for the stringly typed API

Swift 3 brought a tsunami of changes to the language as well as our codebase, some of you reading this may even still be battling with the migration too. But even with all these changes, we’re still left with some  APIs within Foundation that are stringly typed, which is totally fine… Until it’s not.

Read the full article on [Medium](https://medium.com/@AndyyHope)

--

tl;dr:
Turn these

```swift
// Set
UserDefaults.standard.set(true, forKey: Constants.Account.isUserLoggedIn.rawValue)

// Get
UserDefaults.standard.bool(forKey: Constants.Account.isUserLoggedIn.rawValue)
```

Into this

```swift
// Set
UserDefaults.Account.set(true, forKey: .isUserLoggedIn)

// Get
UserDefaults.Account.bool(forKey: .isUserLoggedIn)
```