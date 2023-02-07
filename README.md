# 0x00-AirBnB_clone

## Description
This team project is part of the ALX Full-Stack Software Engineer Programme. It is the first step towards building a first full web application: an AirBnB clone. This first step consists of a custom command-line interface for data management, and the base classes for the storage of this data.

## Usage
The console works both in interactive mode and non-interactive mode, much like a Unix shell. It prints a prompt *(hbnb)* and waits for the user input

## Models
The folder [models](./models) contains all the classes used in this project.


## File Storage
The folder [engine](./models/engine) manages the serialization and deserialization of all the data, following a JSON format.

A FileStorage class is defined in the [file_storage.py](./models/engine/file_storage.py) with methods to follow this flow: `<object> -> to_dict() -> <dictionary> -> JSON dump -> <json string> -> FILE -> <json string> -> JSON load -> <dictionary> -> <object>`

The [init.py](./models/__init__.py) file contains the instantiation of the FileStorage class called *storage*, followed by a call to the method `reload()` on that instance. This allows the storage to be reloaded automatically at initialization which recovers the serialized data.

## Tests
All the code is tested with the *unittest* module. The test for the classes are int the [test_models](./test_models) folder.
