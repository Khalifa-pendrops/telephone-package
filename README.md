# Telephone Package

The Telephone package is a JavaScript module that provides a simple implementation of the Observer pattern for managing phone numbers and notifying observers when a phone number is dialed. 
This package consists of two main classes: `Telephone` and `Observer`.

## Installation

To install the Telephone package, you can use npm:

bash
npm install telephone-package


## Classes

### `Telephone`

The `Telephone` class manages phone numbers and notifies registered observers when a phone number is dialed.

#### Constructor

const telephone = new Telephone(phoneNumbers, observers);


`phoneNumbers`: An optional array to initialize the list of phone numbers.
`observers`: An optional array to initialize the list of observers.

#### Methods

##### `addObserver(observer)`
Adds an observer to the list of observers.

##### `removeObserver(observer)`
Removes an observer from the list of observers.

##### `notifyObservers(number)`
Notifies all observers with the dialed phone number.

##### `addPhoneNumber(number)`
Adds a phone number to the list of phone numbers if it doesn't exist.

##### `removePhoneNumber(number)`
Removes a phone number from the list of phone numbers.

##### `dialPhoneNumber(number)`
Dials the specified phone number, notifying observers if it exists.

### `Observer`

The `Observer` class represents an observer that can be notified when a phone number is dialed.

#### Constructor

const observer = new Observer(name);


`name`: The name of the observer.

#### Methods

##### `notify(number)`
Notifies the observer with the dialed phone number.


## Note
Modify the code as needed for additional functionality or adapt it to suit specific requirements.
This package is intended for educational purposes or as a starting point for more complex implementations.
