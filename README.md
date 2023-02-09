# pubspec

A library for manipulating [pubspec](https://www.dartlang.org/tools/pub/pubspec.html) files.

## Usage

A simple usage example:

    import 'package:pubspec/pubspec.dart';

    main() async {
      // load it
      var pubSpec = await PubSpec.load(myDirectory);

      // change the dependencies to a single path dependency on project 'foo'
      var newPubSpec = pubSpec.copy(dependencies: { 'foo': PathReference('../foo') });

      // save it
      await newPubSpec.save(myDirectory);
    }


## Features and bugs

Submit feature requests and report bugs through the [issue tracker].
[tracker]: https://github.com/KinjalDhamat312/FlutterChatBubble/issues
