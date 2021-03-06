[android-components](../../index.md) / [mozilla.components.feature.remotetabs](../index.md) / [RemoteTabsStorageSuggestionProvider](./index.md)

# RemoteTabsStorageSuggestionProvider

`@ExperimentalCoroutinesApi class RemoteTabsStorageSuggestionProvider : `[`SuggestionProvider`](../../mozilla.components.concept.awesomebar/-awesome-bar/-suggestion-provider/index.md) [(source)](https://github.com/mozilla-mobile/android-components/blob/master/components/feature/remotetabs/src/main/java/mozilla/components/feature/remotetabs/RemoteTabsStorageSuggestionProvider.kt#L20)

A [AwesomeBar.SuggestionProvider](../../mozilla.components.concept.awesomebar/-awesome-bar/-suggestion-provider/index.md) implementation that provides suggestions for remote tabs
based on [RemoteTabsFeature](../-remote-tabs-feature/index.md).

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `RemoteTabsStorageSuggestionProvider(remoteTabs: `[`RemoteTabsFeature`](../-remote-tabs-feature/index.md)`, loadUrlUseCase: `[`LoadUrlUseCase`](../../mozilla.components.feature.session/-session-use-cases/-load-url-use-case/index.md)`, icons: `[`BrowserIcons`](../../mozilla.components.browser.icons/-browser-icons/index.md)`? = null)`<br>A [AwesomeBar.SuggestionProvider](../../mozilla.components.concept.awesomebar/-awesome-bar/-suggestion-provider/index.md) implementation that provides suggestions for remote tabs based on [RemoteTabsFeature](../-remote-tabs-feature/index.md). |

### Properties

| Name | Summary |
|---|---|
| [id](id.md) | `val id: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)<br>A unique ID used for identifying this provider. |

### Inherited Properties

| Name | Summary |
|---|---|
| [shouldClearSuggestions](../../mozilla.components.concept.awesomebar/-awesome-bar/-suggestion-provider/should-clear-suggestions.md) | `open val shouldClearSuggestions: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)<br>If true an [AwesomeBar](../../mozilla.components.concept.awesomebar/-awesome-bar/index.md) implementation can clear the previous suggestions of this provider as soon as the user continues to type. If this is false an [AwesomeBar](../../mozilla.components.concept.awesomebar/-awesome-bar/index.md) implementation is allowed to keep the previous suggestions around until the provider returns a new list of suggestions for the updated text. |

### Functions

| Name | Summary |
|---|---|
| [onInputChanged](on-input-changed.md) | `suspend fun onInputChanged(text: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`): `[`List`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)`<`[`Suggestion`](../../mozilla.components.concept.awesomebar/-awesome-bar/-suggestion/index.md)`>`<br>Fired whenever the user changes their input, after they have started interacting with the awesome bar. |

### Inherited Functions

| Name | Summary |
|---|---|
| [onInputCancelled](../../mozilla.components.concept.awesomebar/-awesome-bar/-suggestion-provider/on-input-cancelled.md) | `open fun onInputCancelled(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Fired when the user has cancelled their interaction with the awesome bar. |
| [onInputStarted](../../mozilla.components.concept.awesomebar/-awesome-bar/-suggestion-provider/on-input-started.md) | `open fun onInputStarted(): `[`List`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)`<`[`Suggestion`](../../mozilla.components.concept.awesomebar/-awesome-bar/-suggestion/index.md)`>`<br>Fired when the user starts interacting with the awesome bar by entering text in the toolbar. |

### Extension Functions

| Name | Summary |
|---|---|
| [loadResourceAsString](../../mozilla.components.support.test.file/kotlin.-any/load-resource-as-string.md) | `fun `[`Any`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)`.loadResourceAsString(path: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`): `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)<br>Loads a file from the resources folder and returns its content as a string object. |
