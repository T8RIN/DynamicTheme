# DynamicTheme

Simple library that allows you to add dynamic theme implementation from android 5 and above to your compose project.

# Examples
## See [ImageResizer](https://github/t8rin/imageResizer)

https://user-images.githubusercontent.com/52178347/229303690-ec7ad907-b06e-4677-92fd-478a62141685.mp4


Attention: ColorPicker not included in the package

# Features
* Declaring custom color scheme based on upt to three colors
* Content based colorscheme by providing bitmap
* Dynamic themeing from android 5
* Amoled mode support
* Flexible api to retrieve secondary and tertiary colors from given primary color
* Animating color scheme changes

:fire::fire::fire::fire::fire::fire::fire::fire::fire::fire::fire::fire::fire::fire:

## Usage

### 1. Add dependencies

![latestVersion](https://img.shields.io/github/v/release/t8rin/DynamicTheme)

```groovy
repositories {
  maven { url 'https://jitpack.io' } // Add jitpack
}
dependencies {
  implementation 'com.github.t8rin:dynamictheme:<latest_version>'
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
