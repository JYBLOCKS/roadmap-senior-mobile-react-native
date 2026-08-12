# Senior Mobile Developer — 52-Week Learning Calendar

**Start date:** Monday, August 17, 2026  
**End date:** Sunday, August 15, 2027  
**Primary specialization:** Senior Mobile Software Engineer — React Native / TypeScript  
**Secondary competencies:** Kotlin / Android, Swift / iOS, Backend integration, Mobile architecture, Testing, Performance, CI/CD, App Store and Play Store delivery

---

## 1. Program Goal

The purpose of this calendar is not to become a developer who only knows how to build screens with React Native.

The target profile is:

```text
Senior Mobile Software Engineer
├── React Native / TypeScript
├── Expo / EAS
├── Android / Kotlin
├── iOS / Swift
├── Mobile architecture
├── Offline-first systems
├── Native integrations
├── Performance profiling
├── Security
├── Automated testing
├── CI/CD
└── Production releases
```

At the end of the program, you should be able to design, build, test, debug, profile, deploy, and defend the architecture of a production mobile application.

---

# 2. Strict Rules

## Rule 1 — 70 / 20 / 10

Your study time must follow this ratio:

- **70% building and debugging**
- **20% official documentation and technical reading**
- **10% videos/courses**

Videos are not the main learning activity.

## Rule 2 — No tutorial cloning

A project does not count if you copied the implementation from a tutorial.

You may use tutorials to understand a concept, but the final implementation must be written independently.

## Rule 3 — Every week produces evidence

Every week must produce at least one of the following:

- working feature;
- automated tests;
- architecture decision record;
- performance report;
- debugging report;
- native integration;
- deployment artifact;
- technical write-up.

## Rule 4 — Sunday Gate

Every Sunday you must answer:

1. What did I build?
2. What broke?
3. Why did it break?
4. What architecture decisions did I make?
5. What would I change in production?
6. Can I explain this week's topic without notes?

If the answer to #6 is **no**, repeat the topic before advancing.

## Rule 5 — Every feature needs tests

When applicable, features must have unit, component, integration, or E2E coverage.

## Rule 6 — Mobile-specific thinking

Always evaluate:

- weak networks;
- offline use;
- background execution;
- battery usage;
- memory constraints;
- process death;
- permissions;
- device differences;
- accessibility;
- security;
- app startup;
- rendering performance.

---

# 3. Weekly Study Schedule

Recommended weekly workload: **~16.5 hours**.

| Day | Time | Activity |
|---|---:|---|
| Monday | 19:00–21:00 | Theory + official documentation + selected video |
| Tuesday | 19:00–21:00 | Guided implementation / exercises |
| Wednesday | 19:00–21:00 | Rebuild concept without tutorial |
| Thursday | 19:00–21:00 | Testing + debugging + profiling |
| Friday | 19:00–20:30 | Review + interview questions + notes |
| Saturday | 09:00–13:00 | Main production-style project |
| Sunday | 09:00–12:00 | Project + architecture review + weekly gate |

If a work or personal commitment prevents a session, recover it before Sunday. Do not carry more than one unfinished week into the next phase.

---

# 4. Main Year-Long Project

Use one production-style application throughout the full program.

Recommended project:

```text
School Assist Mobile
├── Authentication
├── Institution
├── Students
├── Educators
├── Guardians
├── Attendance
├── Evaluations
├── Notifications
├── Profile
└── Settings
```

The project evolves with the curriculum.

Final architecture should eventually include:

```text
School Assist Mobile
│
├── Authentication
│   ├── access token
│   ├── refresh token
│   ├── SecureStore
│   └── biometrics
│
├── Data
│   ├── remote API
│   ├── local SQLite database
│   ├── repositories
│   └── sync engine
│
├── Native
│   ├── camera
│   ├── files
│   ├── location
│   ├── notifications
│   ├── deep linking
│   └── background tasks
│
├── Architecture
│   ├── domain
│   ├── application
│   ├── infrastructure
│   └── presentation
│
├── Testing
│   ├── unit
│   ├── component
│   ├── integration
│   └── E2E
│
└── Production
    ├── observability
    ├── CI/CD
    ├── Play Store
    └── App Store / TestFlight
```

---

# 5. Core Technology Stack

```text
React Native
TypeScript
Expo
Expo Router
EAS
Zustand
React Hook Form
Zod
TanStack Query
SQLite
Reanimated
React Native Gesture Handler
FlashList
Jest
React Native Testing Library
Maestro
Detox
Kotlin
Jetpack Compose
Swift
SwiftUI
GitHub Actions
```

---

# PHASE 1 — React Native Fundamentals

**Weeks 1–4**  
**Dates:** August 17 – September 13, 2026

## Phase objective

Build mobile interfaces using React Native correctly, understand how it differs from React DOM, handle navigation and forms, and produce the first tested application.

## Mandatory resources

- Expo documentation: https://docs.expo.dev/
- React Native documentation: https://reactnative.dev/docs/getting-started
- React Native debugging: https://reactnative.dev/docs/debugging
- Expo Router: https://docs.expo.dev/router/introduction/
- Video — Create your first Expo app: https://www.youtube.com/watch?v=m1-bc53EGh8
- Video — Expo Router navigation: https://www.youtube.com/watch?v=8336fcFV_T4

---

## Week 1 — August 17–23

### Learn

- React Native vs React DOM
- Metro bundler
- Expo development workflow
- `View`
- `Text`
- `Image`
- `Pressable`
- `ScrollView`
- `SafeAreaView`
- `StyleSheet`
- Flexbox on mobile
- `Dimensions`
- `PixelRatio`
- `Platform`
- keyboard basics
- status bar basics

### Build

Create a small multi-screen UI containing:

- home;
- profile;
- cards;
- lists;
- images;
- buttons;
- loading states.

### Deliverable

`week-01-react-native-foundations`

### Sunday Gate

Explain why React Native components are not DOM elements and how layout differs from the web.

---

## Week 2 — August 24–30

### Learn

- Expo Router
- Stack navigation
- Tabs
- Modals
- Nested layouts
- Route parameters
- Typed routes
- Protected route concepts
- Deep-link foundations
- Back navigation

### Build

Create:

```text
/app
├── _layout.tsx
├── index.tsx
├── login.tsx
├── profile.tsx
└── (tabs)/
    ├── _layout.tsx
    ├── home.tsx
    └── settings.tsx
```

### Deliverable

Working navigation architecture with at least one modal and one nested layout.

### Sunday Gate

Draw your navigation tree from memory.

---

## Week 3 — August 31–September 6

### Learn

- React Hook Form
- Zod
- mobile inputs
- focus management
- keyboard handling
- form validation
- accessibility labels
- error messages
- loading and disabled states

### Build

- Login
- Register
- Forgot Password
- Profile
- Change Password

### Deliverable

Reusable form components with tests.

### Sunday Gate

Explain controlled vs uncontrolled inputs and why React Hook Form is useful on mobile.

---

## Week 4 — September 7–13

# PHASE EXAM 1

Build a **Mobile Banking Demo** without following a tutorial.

### Requirements

```text
Authentication
├── Login
├── Protected routes
└── Logout

Home
├── Account balance
├── Transactions
└── Profile

Transfer
├── Form
├── Validation
└── Confirmation modal
```

Use:

- TypeScript
- Expo Router
- React Hook Form
- Zod
- Zustand
- Jest / React Native Testing Library

### Pass criteria

- app runs correctly;
- navigation is typed;
- no major TypeScript errors;
- forms validate properly;
- critical behavior has tests;
- code is organized by responsibility.

---

# PHASE 2 — Networking, Authentication and Architecture

**Weeks 5–8**  
**Dates:** September 14 – October 11, 2026

## Week 5 — September 14–20

### Learn

- HTTP fundamentals
- REST
- Fetch API
- Axios concepts
- timeout
- cancellation
- `AbortController`
- retries
- pagination
- infinite queries
- network errors
- connectivity states
- TanStack Query

### Architecture rule

```text
Server State → TanStack Query
Client State → Zustand
Form State   → React Hook Form
```

### Build

Connect the app to a real API.

### Deliverable

Reusable API client + error normalization layer.

---

## Week 6 — September 21–27

### Learn

Production authentication:

- access tokens
- refresh tokens
- token expiration
- SecureStore
- refresh rotation
- session restoration
- `401` handling
- logout
- protected routes
- authentication race conditions

Official reference:

- https://docs.expo.dev/router/advanced/authentication/

### Build

Implement a complete session lifecycle.

### Deliverable

Authentication module with tests for expiration and refresh behavior.

---

## Week 7 — September 28–October 4

### Learn

- Clean Architecture concepts
- feature-based architecture
- Repository Pattern
- adapters
- dependency inversion
- domain models
- DTO mapping
- service boundaries
- separation of concerns

### Target structure

```text
src/
├── app/
├── features/
│   └── authentication/
│       ├── api/
│       ├── components/
│       ├── hooks/
│       ├── schemas/
│       ├── store/
│       └── types/
├── shared/
├── infrastructure/
└── domain/
```

### Deliverable

Architecture Decision Record explaining your chosen project structure.

---

## Week 8 — October 5–11

# PHASE EXAM 2

Build an **API-driven mobile e-commerce app**.

### Required features

- authentication;
- products;
- search;
- pagination;
- favorites;
- shopping cart;
- profile;
- checkout simulation.

### Pass criteria

- clean separation of state responsibilities;
- API error handling;
- loading / empty / retry states;
- tests;
- documented architecture.

---

# PHASE 3 — Mobile Platform Fundamentals

**Weeks 9–12**  
**Dates:** October 12 – November 8, 2026

## Week 9 — October 12–18

### Learn

Application lifecycle:

```text
Foreground
Background
Inactive
Terminated
```

Also study:

- AppState
- process death
- screen lifecycle
- interruptions
- orientation
- memory pressure
- Android Activity lifecycle
- iOS lifecycle concepts

Android lifecycle reference:

https://developer.android.com/guide/components/activities/activity-lifecycle

### Deliverable

A demo that persists and restores state correctly after lifecycle changes.

---

## Week 10 — October 19–25

### Learn

Device APIs:

- camera
- photo library
- file system
- clipboard
- sharing
- contacts
- location
- permissions

### Build

Create a device-capabilities playground app.

### Deliverable

Permission handling for both accepted and rejected permissions.

---

## Week 11 — October 26–November 1

### Learn

Mobile security:

- SecureStore
- biometrics
- Face ID
- fingerprint
- token storage
- secrets
- permission minimization
- HTTPS concepts
- certificate concepts
- sensitive logging
- screenshots / app switcher considerations

### Deliverable

Security checklist for the main app.

---

## Week 12 — November 2–8

# PHASE EXAM 3

Build **Secure Notes**.

### Required features

- login;
- biometric unlock;
- camera;
- local storage;
- secure secret storage;
- app lock after backgrounding;
- file attachment;
- share functionality.

### Pass criteria

You can explain where sensitive information is stored and why.

---

# PHASE 4 — Offline-First Architecture

**Weeks 13–16**  
**Dates:** November 9 – December 6, 2026

## Week 13 — November 9–15

### Learn SQLite

- tables
- indexes
- migrations
- constraints
- transactions
- queries
- pagination
- schema evolution

### Build

Add a local database to the main app.

### Deliverable

Migration system + repository abstraction.

---

## Week 14 — November 16–22

### Learn offline-first principles

```text
UI
 ↓
Repository
 ↙      ↘
Local DB  Remote API
```

Study:

- source of truth;
- local writes;
- pending mutations;
- stale data;
- cache invalidation;
- connectivity changes.

### Deliverable

At least one feature that works fully offline.

---

## Week 15 — November 23–29

### Learn synchronization

- sync queue
- optimistic updates
- retries
- exponential backoff
- timestamps
- idempotency
- conflict detection
- conflict resolution
- duplicate prevention

### Implement

```text
UI write
   ↓
Local DB
   ↓
pending_operation
   ↓
sync worker
   ↓
API
   ↓
server confirmation
```

### Deliverable

Working synchronization queue.

---

## Week 16 — November 30–December 6

# PHASE EXAM 4

### Test

1. Disable Internet.
2. Create and edit data.
3. Close/reopen app.
4. Verify data remains accessible.
5. Restore Internet.
6. Synchronize data.
7. Force one conflict.
8. Resolve conflict correctly.

### Pass criteria

No silent data loss.

---

# PHASE 5 — Push Notifications and Background Work

**Weeks 17–20**  
**Dates:** December 7, 2026 – January 3, 2027

## Week 17 — December 7–13

### Learn push infrastructure

- APNs
- FCM
- Expo Push Service
- device tokens
- notification permission lifecycle
- token registration
- notification payloads

Official reference:

https://docs.expo.dev/push-notifications/push-notifications-setup/

### Deliverable

Register a physical device and receive a remote notification.

---

## Week 18 — December 14–20

### Learn notification UX

- foreground notification
- background notification
- terminated-state notification
- notification categories
- deep links from notifications
- notification preferences

### Deliverable

Notification opens the correct screen using a deep link.

---

## Week 19 — December 21–27

### Learn background work

- background tasks
- background fetch
- scheduled work
- Android restrictions
- iOS restrictions
- battery impact
- reliability expectations

### Deliverable

Implement one safe background job and document its platform limitations.

---

## Week 20 — December 28–January 3

# PHASE EXAM 5

Build an appointment flow:

```text
Book appointment
      ↓
Backend
      ↓
Push notification
      ↓
Open notification
      ↓
Deep link
      ↓
Appointment detail
```

### Pass criteria

Works in foreground and background states on a real device.

---

# PHASE 6 — Animations and Gestures

**Weeks 21–24**  
**Dates:** January 4 – January 31, 2027

## Mandatory resource

React Native Reanimated:

https://docs.swmansion.com/react-native-reanimated/

---

## Week 21 — January 4–10

### Learn

- React Native Gesture Handler
- tap
- pan
- long press
- gesture composition
- gesture conflicts

### Build

Swipeable card interactions.

---

## Week 22 — January 11–17

### Learn Reanimated

- shared values
- worklets
- UI thread
- `withTiming`
- `withSpring`
- interpolation

### Build

Animated controls and transitions.

---

## Week 23 — January 18–24

### Build

- draggable bottom sheet;
- animated tabs;
- parallax effect;
- collapsible header;
- gesture carousel.

### Deliverable

Animation playground with performance notes.

---

## Week 24 — January 25–31

# PHASE EXAM 6

Build one polished interaction-heavy screen without third-party UI templates.

### Pass criteria

- gestures do not conflict;
- animations remain smooth;
- expensive work does not block the JS thread;
- accessibility remains usable.

---

# PHASE 7 — Mobile Performance Engineering

**Weeks 25–28**  
**Dates:** February 1 – February 28, 2027

## Week 25 — February 1–7

### Learn runtime model

- JS thread
- UI thread
- React render
- React commit
- bridge history
- JSI overview
- dropped frames
- frame budget
- 60 Hz / 120 Hz devices

### Deliverable

Write a short document explaining how a frame reaches the screen.

---

## Week 26 — February 8–14

### Learn profiling

- React Native DevTools
- React Profiler
- Android Studio Profiler
- Xcode Instruments
- CPU profiling
- memory profiling
- network profiling

React Native DevTools:

https://reactnative.dev/docs/react-native-devtools

### Deliverable

Profile one existing feature and identify at least three measurable issues.

---

## Week 27 — February 15–21

### Learn list performance

- FlatList
- virtualization
- windowing
- recycling
- FlashList
- `getItemType`
- stable keys
- memoization
- image performance

FlashList:

https://shopify.github.io/flash-list/docs/

### Deliverable

Benchmark FlatList vs FlashList for a large data set.

---

## Week 28 — February 22–28

# PHASE EXAM 7

Create a screen with:

```text
10,000 messages
images
avatars
dynamic heights
live updates
```

### Pass criteria

Produce a short performance report containing:

- initial metrics;
- bottlenecks;
- optimizations;
- final metrics;
- explanation of trade-offs.

Never optimize without measuring.

---

# PHASE 8 — Native Android and Kotlin

**Weeks 29–34**  
**Dates:** March 1 – April 11, 2027

## Mandatory resources

- Android courses: https://developer.android.com/courses
- Android Basics with Compose: https://developer.android.com/courses/android-basics-compose/course
- Android architecture pathway: https://developer.android.com/courses/pathways/android-architecture
- Video — Thinking in Compose: https://www.youtube.com/watch?v=SMOhl9RK0BA

---

## Week 29 — March 1–7

### Kotlin fundamentals

- `val` / `var`
- functions
- nullability
- classes
- data classes
- interfaces
- enums
- sealed classes

### Deliverable

Kotlin exercises without Android.

---

## Week 30 — March 8–14

### Advanced Kotlin

- generics
- extensions
- lambdas
- collections
- higher-order functions
- scope functions

### Deliverable

Small Kotlin domain module with tests.

---

## Week 31 — March 15–21

### Kotlin concurrency

- coroutines
- `suspend`
- structured concurrency
- Flow
- StateFlow
- error handling
- cancellation

### Deliverable

Async repository demo.

---

## Week 32 — March 22–28

### Android fundamentals

- Activity
- lifecycle
- Manifest
- Intent
- permissions
- Android Studio
- Gradle

### Deliverable

Simple native Android app.

---

## Week 33 — March 29–April 4

### Jetpack Compose

- composables
- state
- recomposition
- navigation
- ViewModel
- StateFlow integration
- Material concepts

### Deliverable

Three-screen Compose app.

---

## Week 34 — April 5–11

# PHASE EXAM 8

Build a **100% Kotlin + Jetpack Compose** application.

### Must include

- navigation;
- API call;
- ViewModel;
- Flow / StateFlow;
- local persistence;
- loading/error states;
- tests.

**React Native is not allowed during this exam.**

---

# PHASE 9 — Native iOS and Swift

**Weeks 35–40**  
**Dates:** April 12 – May 23, 2027

## Mandatory Apple resources

- Demystify SwiftUI: https://developer.apple.com/videos/play/wwdc2021/10022/
- Embracing Swift Concurrency: https://developer.apple.com/videos/play/wwdc2025/268/
- Explore concurrency in SwiftUI: https://developer.apple.com/videos/play/wwdc2025/266/
- Code-along — Swift concurrency: https://developer.apple.com/videos/play/wwdc2025/270/

---

## Week 35 — April 12–18

### Swift fundamentals

- `let` / `var`
- functions
- structs
- classes
- enums
- optionals
- `guard`

### Deliverable

Swift exercises without SwiftUI.

---

## Week 36 — April 19–25

### Advanced Swift

- protocols
- extensions
- closures
- generics
- error handling
- value vs reference semantics

### Deliverable

Small domain module with tests.

---

## Week 37 — April 26–May 2

### Swift concurrency

- async/await
- Task
- cancellation
- actors
- MainActor

### Deliverable

Concurrent networking demo.

---

## Week 38 — May 3–9

### SwiftUI fundamentals

- View
- State
- Binding
- Observable
- Environment
- NavigationStack
- List
- Sheet

### Deliverable

Three-screen SwiftUI application.

---

## Week 39 — May 10–16

### Xcode / iOS platform

- Xcode projects
- schemes
- targets
- simulator
- device deployment
- Info.plist
- capabilities
- certificates
- provisioning profiles
- Instruments

### Deliverable

Run the app on a physical device if available.

---

## Week 40 — May 17–23

# PHASE EXAM 9

Build a **100% Swift + SwiftUI** application.

### Must include

- navigation;
- API call;
- async/await;
- local persistence;
- loading/error states;
- tests.

**React Native is not allowed during this exam.**

---

# PHASE 10 — React Native Internals and Native Modules

**Weeks 41–44**  
**Dates:** May 24 – June 20, 2027

## Mandatory references

- New Architecture: https://reactnative.dev/architecture/landing-page
- Hermes: https://reactnative.dev/docs/hermes
- Codegen: https://reactnative.dev/docs/the-new-architecture/using-codegen
- Turbo Native Modules: https://reactnative.dev/docs/next/turbo-native-modules-introduction

---

## Week 41 — May 24–30

### Learn

- old bridge architecture
- New Architecture
- JSI
- why synchronous native access matters
- C++ layer concepts

### Required diagram

Draw from memory:

```text
JavaScript / TypeScript
        │
        │ JSI
        ▼
    C++ Runtime
   /           \
TurboModules   Fabric
     │           │
 Native APIs   Native UI
```

---

## Week 42 — May 31–June 6

### Learn Hermes

- JavaScript engine role
- bytecode concepts
- startup time
- memory
- garbage collection concepts
- profiling

### Deliverable

Technical note: "What Hermes changes in a React Native app".

---

## Week 43 — June 7–13

### Learn

- Fabric
- TurboModules
- Codegen
- typed native specifications
- native component architecture

### Deliverable

Create a small native specification.

---

## Week 44 — June 14–20

# PHASE EXAM 10

Build a custom React Native native module.

```text
TypeScript API
     │
     ├── Android → Kotlin
     └── iOS     → Swift
```

### Possible module ideas

- battery/device diagnostics;
- native secure utility;
- custom sensor wrapper;
- system information;
- custom native UI component.

### Pass criteria

You can explain the path from TypeScript call to native implementation.

---

# PHASE 11 — Professional Testing

**Weeks 45–48**  
**Dates:** June 21 – July 18, 2027

## Required tools

- Jest
- React Native Testing Library
- Maestro
- Detox

References:

- Expo E2E / Maestro: https://docs.expo.dev/eas/workflows/examples/e2e-tests/
- Detox: https://wix.github.io/Detox/docs/introduction/getting-started/
- Video — E2E tests on EAS Build: https://www.youtube.com/watch?v=-o-bfIRrg9U

---

## Week 45 — June 21–27

### Unit testing

Test:

- domain rules;
- validation;
- repositories;
- state transitions;
- synchronization logic.

### Deliverable

Critical domain unit-test suite.

---

## Week 46 — June 28–July 4

### Component and integration testing

Use React Native Testing Library.

Test:

- forms;
- user interactions;
- error states;
- loading states;
- navigation-related behavior.

### Deliverable

Integration suite for one complete feature.

---

## Week 47 — July 5–11

### E2E testing

Learn Maestro.

Automate:

```text
Login
→ navigate
→ create record
→ verify record
→ edit record
→ logout
```

### Deliverable

Working E2E flow.

---

## Week 48 — July 12–18

# PHASE EXAM 11

Add a complete test strategy to the main project.

```text
           E2E
          /   \
     Integration
       /       \
    Unit     Component
```

### Required documentation

Explain which tests belong at each layer and what you deliberately do **not** test.

---

# PHASE 12 — CI/CD, Distribution and Production

**Weeks 49–52**  
**Dates:** July 19 – August 15, 2027

## Mandatory references

- EAS Workflows: https://docs.expo.dev/eas/workflows/introduction/
- EAS Build: https://docs.expo.dev/build/introduction/
- Expo development builds: https://www.youtube.com/watch?v=FdjczjkwQKE
- Configure development build with EAS: https://www.youtube.com/watch?v=uQCE9zl3dXU

---

## Week 49 — July 19–25

### Learn CI/CD basics

- GitHub Actions
- EAS Workflows
- environment separation
- secrets
- build profiles
- preview builds
- staging
- production

### Build pipeline

```text
Pull Request
    ↓
Lint
    ↓
Type Check
    ↓
Unit Tests
    ↓
Integration Tests
    ↓
Build
```

### Deliverable

CI pipeline running on every PR.

---

## Week 50 — July 26–August 1

### Learn release systems

- EAS Build
- development builds
- preview builds
- production builds
- signing concepts
- Android keystore
- iOS certificates
- provisioning

### Deliverable

Installable Android and iOS builds.

---

## Week 51 — August 2–8

### Learn production updates

- EAS Update
- OTA updates
- release channels
- runtime versions
- semantic versioning
- rollback strategy
- observability
- crash reporting concepts

### Deliverable

Documented release and rollback procedure.

---

## Week 52 — August 9–15

# FINAL EXAM — PRODUCTION RELEASE

Publish or distribute the final application.

Minimum target:

```text
Android
└── Play Console internal / closed testing or production

Apple
└── TestFlight and App Store submission path
```

### Final production checklist

- [ ] lint passes
- [ ] TypeScript passes
- [ ] unit tests pass
- [ ] component tests pass
- [ ] integration tests pass
- [ ] E2E critical path passes
- [ ] offline behavior verified
- [ ] error states verified
- [ ] analytics/observability strategy exists
- [ ] secrets are not committed
- [ ] privacy permissions documented
- [ ] push notifications tested
- [ ] deep links tested
- [ ] performance profiled
- [ ] Android release build generated
- [ ] iOS release build generated
- [ ] CI/CD pipeline working
- [ ] release documentation complete

---

# 6. Senior Gate — Required Knowledge

At the end of the 52 weeks, answer all of these without searching first.

## React Native

- [ ] How does React Native render UI?
- [ ] What is JSI?
- [ ] What problem did the old bridge have?
- [ ] What is Fabric?
- [ ] What are TurboModules?
- [ ] What does Codegen do?
- [ ] Why does React Native use Hermes?
- [ ] JS thread vs UI thread?
- [ ] What causes dropped frames?
- [ ] What causes unnecessary re-renders?

## Performance

- [ ] How do you profile a React Native application?
- [ ] When should you use `React.memo`?
- [ ] When can memoization hurt?
- [ ] FlatList vs FlashList?
- [ ] How would you render 50,000 records?
- [ ] How do you detect a memory leak?
- [ ] How do you reduce startup time?

## Architecture

- [ ] How would you design an offline-first app?
- [ ] What is the source of truth?
- [ ] How do you synchronize offline mutations?
- [ ] How do you prevent duplicate mutations?
- [ ] How do you resolve synchronization conflicts?
- [ ] How would you structure a large React Native codebase?
- [ ] When should state live in Zustand vs TanStack Query?

## Security

- [ ] Where should access tokens be stored?
- [ ] Where should refresh tokens be stored?
- [ ] What should never be stored in AsyncStorage?
- [ ] How do biometrics fit into authentication?
- [ ] What happens when a token expires while several requests are running?

## Mobile platform

- [ ] What happens when Android kills the app process?
- [ ] What happens when iOS backgrounds an app?
- [ ] How are permissions handled?
- [ ] How do APNs and FCM work conceptually?
- [ ] How does deep linking work?
- [ ] What limitations exist for background work?

## Android / Kotlin

- [ ] What is an Activity?
- [ ] Explain Android lifecycle.
- [ ] What is a Coroutine?
- [ ] What is structured concurrency?
- [ ] Flow vs StateFlow?
- [ ] What is a ViewModel?
- [ ] How does Compose state trigger recomposition?
- [ ] How does Gradle participate in the build?

## iOS / Swift

- [ ] Struct vs class?
- [ ] What is an Optional?
- [ ] What is a protocol?
- [ ] What is an actor?
- [ ] What is MainActor?
- [ ] How does SwiftUI state work?
- [ ] What are certificates and provisioning profiles?
- [ ] How do you profile an app with Instruments?

## Native integration

- [ ] How would you expose Kotlin code to React Native?
- [ ] How would you expose Swift code to React Native?
- [ ] What role does Codegen have?
- [ ] When would you create a native module rather than use JavaScript?

## Testing

- [ ] Unit vs integration vs E2E?
- [ ] What should be tested with React Native Testing Library?
- [ ] When would you use Maestro?
- [ ] When would you use Detox?
- [ ] How do you prevent flaky E2E tests?

## Production

- [ ] How do Android release builds work?
- [ ] How do iOS release builds work?
- [ ] How would you implement CI/CD?
- [ ] What is an OTA update?
- [ ] When is an OTA update unsafe?
- [ ] How would you perform rollback?
- [ ] How would you monitor crashes and regressions?

If you cannot explain one of these topics, add it back to the study backlog.

---

# 7. Monthly Retrospective

At the end of every four weeks, create:

```text
reports/
└── YYYY-MM-mobile-retrospective.md
```

Answer:

1. What concepts can I explain confidently?
2. Which concepts can I use but not explain?
3. Which bugs took me longest to solve?
4. Which architecture decision was hardest?
5. Where did I over-engineer?
6. Where did I under-engineer?
7. What is my weakest topic right now?
8. Which feature would I be comfortable defending in a senior interview?
9. Which feature would I not be comfortable defending?
10. What do I need to repeat next month?

---

# 8. Required Portfolio Evidence

By the end of the program, your GitHub/portfolio should demonstrate more than UI screenshots.

## Minimum evidence

- [ ] one production-grade React Native application
- [ ] one small Kotlin / Jetpack Compose app
- [ ] one small Swift / SwiftUI app
- [ ] one custom React Native native module
- [ ] offline-first architecture
- [ ] synchronization engine
- [ ] push notifications
- [ ] deep links
- [ ] biometric authentication
- [ ] camera/file integration
- [ ] local SQLite persistence
- [ ] performance report
- [ ] testing strategy
- [ ] E2E tests
- [ ] CI/CD pipeline
- [ ] architecture decision records
- [ ] release documentation
- [ ] Android distribution
- [ ] iOS/TestFlight distribution path

---

# 9. Recommended Repository Documentation

Maintain these files in the main project:

```text
/docs
├── architecture/
│   ├── architecture-overview.md
│   ├── offline-first.md
│   ├── authentication.md
│   ├── notifications.md
│   └── native-modules.md
│
├── decisions/
│   ├── ADR-001-state-management.md
│   ├── ADR-002-server-state.md
│   ├── ADR-003-local-database.md
│   ├── ADR-004-sync-strategy.md
│   └── ADR-005-navigation.md
│
├── performance/
│   ├── list-benchmark.md
│   └── startup-profile.md
│
├── testing/
│   └── testing-strategy.md
│
└── production/
    ├── release-process.md
    └── rollback.md
```

This documentation becomes part of your senior-level portfolio because it demonstrates reasoning, not only implementation.

---

# 10. Interview Practice Routine

Starting in **Week 13**, every Friday spend at least 20 minutes answering technical questions aloud.

Use this format:

```text
Problem
→ constraints
→ possible solutions
→ chosen solution
→ trade-offs
→ failure modes
→ observability
→ testing
```

Example:

> Design an offline-first attendance system for a school where teachers may lose connectivity for several hours.

A senior answer should discuss data ownership, local persistence, sync, conflict resolution, retries, idempotency, visibility to the user, observability, and failure recovery.

---

# 11. Definition of Done for the Program

The roadmap is finished only when all of the following are true:

- [ ] 52 weeks completed
- [ ] all phase exams passed
- [ ] React Native fundamentals mastered
- [ ] production authentication implemented
- [ ] offline-first flow implemented
- [ ] native device APIs implemented
- [ ] push notifications implemented
- [ ] deep linking implemented
- [ ] background work understood and tested
- [ ] animations/gestures implemented
- [ ] performance profiling performed
- [ ] Android Kotlin application built
- [ ] iOS Swift application built
- [ ] custom RN native module built
- [ ] unit tests implemented
- [ ] integration tests implemented
- [ ] E2E tests implemented
- [ ] CI/CD implemented
- [ ] Android release produced
- [ ] iOS/TestFlight release path completed
- [ ] Senior Gate answered confidently
- [ ] main project documented

---

# Final Target

By August 15, 2027, your target profile is:

```text
Senior Mobile Software Engineer
React Native / TypeScript

Native
├── Kotlin / Android
└── Swift / iOS

Architecture
├── Offline-first
├── Clean Architecture
├── Repository Pattern
├── Native Modules
├── Secure Authentication
└── Sync Engines

Performance
├── Hermes
├── JSI
├── Fabric
├── TurboModules
├── Codegen
└── Profiling

Testing
├── Jest
├── React Native Testing Library
├── Maestro
└── Detox

Production
├── Expo / EAS
├── GitHub Actions
├── Play Store
└── App Store / TestFlight

Backend Integration
├── REST
├── WebSockets
├── FastAPI / Node
└── PostgreSQL
```

The objective is not to memorize this stack. The objective is to be able to **design, implement, debug, measure, test, release, and explain it**.

---

# Start

**Monday, August 17, 2026 — Week 1, Day 1**

First task:

```text
Create the React Native workspace.
Configure TypeScript.
Run the app on Android and iOS environments where available.
Create the first screen without copying a tutorial.
Commit the result.
```

Recommended first commit:

```text
chore: initialize mobile learning project
```

Then begin Week 1.
