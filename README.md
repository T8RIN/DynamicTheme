
<h1 align="center">

DynamicTheme

</h1>


<p align="center">
 <img alt="material" src="https://custom-icon-badges.demolab.com/badge/material%20you-palegreen?style=for-the-badge&logoColor=black&logo=material-you"/></a>
  <img alt="API" src="https://img.shields.io/badge/Api%2021+-50f270?logo=android&logoColor=black&style=for-the-badge"/></a>
  <img alt="Kotlin" src="https://img.shields.io/badge/Kotlin-a503fc?logo=kotlin&logoColor=white&style=for-the-badge"/></a>
  <img alt="Jetpack Compose" src="https://img.shields.io/static/v1?style=for-the-badge&message=Jetpack+Compose&color=4285F4&logo=Jetpack+Compose&logoColor=FFFFFF&label="/></a> 
  <a href="https://hits.sh/github.com/t8rin/dynamictheme/"><img alt="Hits" src="https://hits.sh/github.com/t8rin/dynamictheme.svg?style=for-the-badge&label=Views&extraCount=10&color=54856b"/></a>
</p>


<p align="center">🎨 Jetpack Compose material theming library, which falls back onto a custom dynamic colors implementation based on wallpapers to support older API levels.
Yes! Dynamic colors are now available even on old android devices, enjoy!</p>

# Examples (See [ImageResizer](https://github.com/t8rin/imageResizer))

<p align="center">
 <img alt="material" src="https://user-images.githubusercontent.com/52178347/229307585-a0c871f7-0bb8-43da-a7c7-cf1c41d6d35f.gif" width="36.6%"/></a>
  <img alt="API" src="https://user-images.githubusercontent.com/52178347/229358462-560e987b-e401-446a-b791-c9a0fb93f8e8.jpg" width="30%"/></a>
  <img alt="Kotlin" src="https://user-images.githubusercontent.com/52178347/229358471-5709401a-7518-4323-8f5c-b4e9b5a3bf5c.jpg" width="30%"/></a></a> 
</p>


Attention: ColorPicker not included in the package

# Features
* Declaring custom color scheme based on up to three colors
* Content based colorscheme by providing bitmap
* Dynamic themeing from android 5
* Amoled mode support
* Flexible api to retrieve secondary and tertiary colors from given primary color
* Animating color scheme changes

:fire::fire::fire::fire::fire::fire::fire::fire::fire::fire::fire::fire::fire::fire:

## Usage

### 1. Add dependencies

![latestVersion](https://img.shields.io/github/v/release/t8rin/DynamicTheme?style=for-the-badge)

#### Kotlin (kts)
```kotlin
repositories {
  maven { setUrl("https://jitpack.io") } // Add jitpack
}
dependencies {
  implementation("com.github.t8rin:dynamictheme:LATEST_VERSION") // Replace "LATEST_VERSION" with preferrend version tag
}
```

#### Groovy
```groovy
repositories {
  maven { url 'https://jitpack.io' } // Add jitpack
}
dependencies {
  implementation 'com.github.t8rin:dynamictheme:LATEST_VERSION' // Replace "LATEST_VERSION" with preferrend version tag
}
```

### 2. Add `DynamicTheme` call

```kotlin
@Composable
fun DynamicThemeComposable() {

    DynamicTheme(
        state = rememberDynamicThemeState(),
        defaultColorTuple = ColorTuple(
            primary = /*your value*/,
            secondary = /*your value (optional)*/,
            tertiary = /*your value (optional)*/
        ),
        content = {
            /*your content
            * there you can get you provided state value by LocalDynamicThemeState.current
            */
        }
    )
    
    //...
    // Also you can use ColorTupleItem to get represenation of your color scheme by three colors
```

## Roadmap
- [ ] Rewrite to Kotlin

## Find this repository useful? :heart:
Support it by joining __[stargazers](https://github.com/t8rin/DynamicTheme/stargazers)__ for this repository. :star: <br>
And __[follow](https://github.com/t8rin)__ me for my next creations! 🤩

# License
```xml
Designed and developed by 2023 T8RIN

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
