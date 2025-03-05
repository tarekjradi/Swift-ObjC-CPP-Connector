# Swift-Objective-C-CPP-Bridge

The **Swift-Objective-C-CPP-Bridge** project enables seamless interoperability between Swift, Objective-C, and C++ by providing a simple bridging mechanism. It allows developers to call C++ functions and use C++ classes directly from Swift and Objective-C code, making it easier to integrate legacy C++ codebases into modern Swift applications.

## Aim

The primary goal of this project is to provide a straightforward and efficient way to enable **cross-language communication** between Swift, Objective-C, and C++ components. Whether you're working with legacy C++ code, trying to integrate Objective-C libraries, or building a hybrid Swift project, this bridge allows you to combine the power of all three languages in a clean and maintainable way.

## Features

- **C++ and Swift Interoperability**: Easily call C++ methods from Swift code.
- **Objective-C Bridging**: Use C++ and Swift code within Objective-C projects.
- **Simple Integration**: Minimal boilerplate and configuration needed for bridging.

## Example Usage

### Swift Code Example

In your Swift code, you can call the `add` function from the C++ class `Operators` by using the Objective-C bridge class `CppBridging`. Here's an example:

```swift
import SwiftUI

struct ContentView: View {
    var body: some View {
        Text("\(CppBridging.add(10, b: 5))")
            .padding()
    }
}

struct ContentView_Previews: PreviewProvider {
    static var previews: some View {
        ContentView()
    }
}
