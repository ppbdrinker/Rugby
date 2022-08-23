<br>
<p align="center">
  <img src="https://user-images.githubusercontent.com/64660122/140398205-9328806e-897d-483d-a898-c90f66840196.png" width="600"/>
</p>
<p align="center">
  <img src="https://user-images.githubusercontent.com/64660122/141674975-22c970d6-943e-49cc-a86a-42276b3520e8.mp4" width="600"/>
</p>
<p align="center">
  <a href="https://swiftpackageindex.com/swiftyfinch/Rugby"><img src="https://img.shields.io/endpoint?color=orange&label=Swift&logo=swift&logoColor=white&url=https%3A%2F%2Fswiftpackageindex.com%2Fapi%2Fpackages%2Fswiftyfinch%2FRugby%2Fbadge%3Ftype%3Dswift-versions" /></a>
  <a href="https://swiftpackageindex.com/swiftyfinch/Rugby"><img src="https://img.shields.io/endpoint?label=Platform&url=https%3A%2F%2Fswiftpackageindex.com%2Fapi%2Fpackages%2Fswiftyfinch%2FRugby%2Fbadge%3Ftype%3Dplatforms" /></a>
  <br>
  <a href="https://brew.sh"><img src="https://img.shields.io/badge/Homebrew-8B4513" /></a>
  <a href="https://github.com/yonaskolb/Mint"><img src="https://img.shields.io/badge/Mint-darkgreen?logo=leaflet&logoColor=white" /></a>
  <a href="https://swiftpackageindex.com/swiftyfinch/Rugby"><img src="https://img.shields.io/badge/Swift_Package_Index-red?logo=swift&logoColor=white" /></a>
  <br>
  <img src="https://img.shields.io/badge/Press_★_for_pay_respect-white?logo=github&logoColor=black" />
  <a href="https://twitter.com/swiftyfinch"><img src="https://img.shields.io/badge/SwiftyFinch-blue?logo=twitter&logoColor=white" /></a>
</p>


### `Motivation`

Working on a project with a huge amount of pods I had some troubles:\
`-` Slow and unnecessary indexing of pods targets, which implementation I rarely try to edit;\
`-` Redundant rebuild time, probably as a result of problems `CocoaPods` hooks or Xcode build system;\
`-` Freezing UI during navigation.

You can read 📖 [full story](https://swiftyfinch.github.io/en/2021-03-09-rugby-story/) on my blog.

### `Description`

🏈 `Rugby` is CLI tool that was developed to solve the above problems:\
`+` Cache all pods dependencies and remove their targets from the Pods project;\
`+` Rebuild only changed pods;\
`+` Remove unnecessary sources from a project and reduce project size;\
`+` Drop any unneeded targets with sources and resources by RegEx.

### `What makes it different?`

🕊 Not a dependency, just an optional step\
🔒 Doesn't change Podfile and Podfile.lock\
🛠 [Custom steps](Docs/Plans.md)\
📈 Metrics after each command\
✨ Fancy log output\
🚀 Swiftish!

Rugby alternatives:\
`-` [PodBuilder](https://github.com/Subito-it/PodBuilder)\
`-` [CocoaPods Binary Cache](https://github.com/grab/cocoapods-binary-cache)\
`-` [CocoaPods Binary](https://github.com/leavez/cocoapods-binary)

### `Discussions`

You can read more about 🏈 Rugby in [`discussions`](https://github.com/swiftyfinch/Rugby/discussions) section.\
Feel free to report any issues or suggest some new feature requests.

### `Known limitations`

`-` Not supported `WatchOS` SDK

<br>

## Download binary with [Homebrew](https://brew.sh) 🍺

```bash
brew tap swiftyfinch/Rugby https://github.com/swiftyfinch/Rugby.git
brew install rugby
```

## Build from source code with <a href="https://github.com/yonaskolb/Mint">Mint</a> 🌱

```bash
brew install mint
mint install swiftyfinch/rugby
```

> **Warning**: Now on **Mint 0.17.0** you'll need to add `~/.mint/bin` to your **$PATH**<br>
> For example, add this to your `~/.zshrc` file and relaunch terminal

```bash
export PATH=$HOME/.mint/bin:$PATH
```
More info about [installation](https://github.com/swiftyfinch/Rugby/discussions/71) with demo 🎬

## How to use 🏈

Run in your project directory after each pod install:
```bash
pod install && rugby
```
Watch 🎬 [Basic Usage Demo](https://github.com/swiftyfinch/Rugby/discussions/72)<br>
Read more [about advanced usage](Docs/Plans.md#-generate-example)

## Documentation 📚

| Command | Description |
| :----- | :------ |
🚑 [`Help`](Docs/README.md) | General Rugby documentation.
🏈 [`Cache`](Docs/Cache.md) | Convert pods to prebuilt dependencies.
✈️ [`Plans`](Docs/Plans.md) | Run a predefined sequence of commands.
🔍 [`Focus`](Docs/Focus.md) | Keep only selected targets and all their dependencies.
🗑 [`Drop`](Docs/Drop.md) | Remove any targets by RegEx.

| 🎓 How To |
| :----- |
🎬 [Installation Demo](https://github.com/swiftyfinch/Rugby/discussions/71)
🎬 [Basic Usage Demo](https://github.com/swiftyfinch/Rugby/discussions/72)
🎬 [Debug Demo](https://github.com/swiftyfinch/Rugby/discussions/142)
🎬 [Rugby Review (ru)](https://github.com/swiftyfinch/Rugby/discussions/146)
<br>

### `Author`

Vyacheslav Khorkov\
Twitter: [@SwiftyFinch](https://twitter.com/swiftyfinch)\
Blog: [swiftyfinch.github.io](https://swiftyfinch.github.io/en)\
Feel free to contact me 📮
