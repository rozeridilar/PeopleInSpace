# PeopleInSpace

Minimal **Kotlin Multiplatform** project using Jetpack Compose and SwiftUI.  Currently running on
* Android
* iOS
* watchOS
* macOS
* Web
* JVM (small Ktor back end service)

It makes use of basic API (http://open-notify.org/Open-Notify-API/People-In-Space/) to show list of people currently in
space (inspired by https://kousenit.org/2019/12/19/a-few-astronomical-examples-in-kotlin/)!  The list is shown on Android
using **Jetpack Compose**, on iOS using **SwiftUI** and on Web using Kotlin/JS React wrapper.

Related posts (please be aware that these were written pre Kotlin 1.4...I plan on updating them soon
to reflect 1.4 changes):
* [Minimal Kotlin Multiplatform project using Compose and SwiftUI](https://johnoreilly.dev/posts/minimal-kotlin-platform-compose-swiftui/)
* [Adding some Storage (to) Space](https://johnoreilly.dev/posts/adding-sqldelight-to-peopleinspace/)
* [Kotlin Multiplatform running on macOS](https://johnoreilly.dev/posts/kotlinmultiplatform-macos/)
* [PeopleInSpace hits the web with Kotlin/JS and React](https://johnoreilly.dev/posts/peopleinspace-kotlinjs/)
* [Using Koin in a Kotlin Multiplatform Project](https://johnoreilly.dev/posts/kotlinmultiplatform-koin/)


Note that this repository very much errs on the side of mimimalism to help more clearly illustrate key moving parts of a Koltin
Multiplatform project and also to hopefully help someone just starting to explore KMP to get up and running for first time (and is of course
primarily focussed on use of Jetpack Compose and SwiftUI).  If you're at stage of moving
beyond this then I'd definitely recommend checking out [KaMPKit](https://github.com/touchlab/KaMPKit)


### Building
You need to use Android Studio v4.2 (currently preview/canary version).  Have tested on XCode v11 and v12 beta.  When opening
iOS/watchOS/macOS projects remember to open `.xcworkspace` file (and not `.xcodeproj` one). To exercise web client run `./gradlew :web:browserDevelopmentRun`.


### Languages, libraries and tools used

* [Kotlin](https://kotlinlang.org/)
* [Kotlin Coroutines](https://kotlinlang.org/docs/reference/coroutines-overview.html)
* [Kotlinx Serialization](https://github.com/Kotlin/kotlinx.serialization)
* [Ktor client library](https://github.com/ktorio/ktor)
* [Android Architecture Components](https://developer.android.com/topic/libraries/architecture/index.html)
* [Koin](https://github.com/InsertKoinIO/koin)
* [Jetpack Compose](https://developer.android.com/jetpack/compose)
* [SwiftUI](https://developer.apple.com/documentation/swiftui)
