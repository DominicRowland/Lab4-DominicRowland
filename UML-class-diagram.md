a# UML Class Diagram - Animal Hierarchy

```mermaid
classDiagram
    class Animal {
        - String name
        + Animal(String name)
        + String getName()
        + String makeSound()
    }
    class Dog {
        - String breed
        + Dog(String name, String breed)
        + String getBreed()
        + String makeSound()
        + void fetch()
    }
    class Cat {
        - int lives
        + Cat(String name)
        + int getLives()
        + void loseLive()
        + String makeSound()
    }
    class Bird {
        - boolean canFly
        + Bird(String name, boolean canFly)
        + boolean getCanFly()
        + String makeSound()
        + void fly()
    }

    Animal <|-- Dog
    Animal <|-- Cat
    Animal <|-- Bird
