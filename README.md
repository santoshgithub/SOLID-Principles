# SOLID-Principles

The SOLID principles are a set of design guidelines for writing maintainable and scalable software. These principles were introduced by Robert C. Martin and are widely recognized as best practices in object-oriented programming. The acronym SOLID stands for the following five principles:

Single Responsibility Principle (SRP): A class should have only one reason to change, meaning that a class should have only one responsibility.
Example: Consider a class "Invoice" that calculates the total amount of an invoice. The SRP states that this class should only be responsible for calculating the total amount, and not for saving the invoice to a database or sending it by email. This can be achieved by splitting the class into two separate classes: "InvoiceCalculator" and "InvoicePersister".

Open/Closed Principle (OCP): Software entities should be open for extension but closed for modification. This means that you should be able to add new functionality to a class without changing its existing code.
Example: Consider a class "Shape" with subclasses "Rectangle", "Triangle", and "Circle". According to the OCP, you should be able to add a new shape, such as "Ellipse", without modifying the "Shape" class. This can be achieved by using inheritance and polymorphism, so that the new "Ellipse" class can extend the "Shape" class and implement the required methods.

Liskov Substitution Principle (LSP): Subtypes must be substitutable for their base types. This means that objects of a derived class should be able to replace objects of the base class without affecting the correctness of the program.
Example: Consider a class "Bird" with a subclass "Penguin". According to the LSP, a method that takes a "Bird" object as a parameter should be able to work with a "Penguin" object without any problems. This can be achieved by ensuring that the "Penguin" class implements all the methods of the "Bird" class and behaves in the same way.

Interface Segregation Principle (ISP): Clients should not be forced to depend on interfaces they do not use. This means that a class should have small, specialized interfaces that are tailored to the needs of its clients.
Example: Consider a class "Printer" that has a method "Print". According to the ISP, a client that only needs to print text should not be forced to depend on a method "PrintImage" that is not needed. This can be achieved by splitting the "Printer" class into two separate interfaces: "TextPrinter" and "ImagePrinter".

Dependency Inversion Principle (DIP): High-level modules should not depend on low-level modules; both should depend on abstractions. This means that you should depend on abstractions, not on concrete implementations.
Example: Consider a class "ReportGenerator" that depends on a class "DataSource" to get data for generating a report. According to the DIP, the "ReportGenerator" class should depend on an interface "IDataSource" instead of the concrete "DataSource" class. This way, you can easily switch to a different implementation of the "IDataSource" interface, such as a "RemoteDataSource", without affecting the "ReportGenerator" class.

By following the SOLID principles, you can create software that is more maintainable, scalable, and flexible.
