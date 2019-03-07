# colorize_lumberdash

Plugin for [lumberdash](https://github.com/jorgecoca/lumberdash)

It prints your logs with different colors on the stdout depending on the severity level

![colorize](../../art/colorized.png)

## How to use

Add `colorize_lumberdash` to your dependencies. Then pass an instance of `ColorizeLumberdash` to `lumberdash`:

```dart
import 'package:colorize_lumberdash/colorize_lumberdash.dart';
import 'package:lumberdash/lumberdash.dart';

void main() {
  putLumberdashToWork(withClient: ColorizeLumberdash());
  logWarning('Hello Warning');
  logFatal('Hello Fatal!');
  logMessage('Hello Message!');
  logError(Exception('Hello Error'));
}
```

## License

```
MIT License

Copyright (c) 2019 Jorge Coca

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```