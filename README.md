# BlurKit
<a href="https://github.com/Carthage/Carthage/"><img src="https://img.shields.io/badge/Carthage-compatible-4BC51D.svg?style=flat"></a>
<img src="https://img.shields.io/badge/platforms-iOS-lightgrey.svg">
<img src="https://img.shields.io/badge/language-Swift%204.2-orange.svg">
<img src="https://img.shields.io/badge/license-MIT-blue.svg">

# Usage
```swift
class ViewController: UIViewController {

    override func viewDidLoad() {
        super.viewDidLoad()
        
        view.bk.addBlur(blurRadius: 0)

        UIView.animate(withDuration: 5) {
            self.view.bk.blurRadius = 5
        }
        
        //  or
        //  label.bk.addBlur(blurRadius: 3, colorTint: .white, colorTintAlpha: 0.4)
        //  imageView.bk.addBlur(blurRadius: 4, colorTint: .white, colorTintAlpha: 0.2)
    }
}
```

# Installation
Add this to `Cartfile`
```
github "touyu/BlurKit" ~> 0.1
```
```
$ carthage update --platform iOS
```
