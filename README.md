# Dependency Injection



> In software engineering, **dependency injection** is a technique whereby one object (or static method) supplies the dependencies of another object. A dependency is an object that can be used (a service).

#### **There are basically three types of dependency injection:**

1. **constructor injection:** the dependencies are provided through a class constructor.
2. **setter injection:** the client exposes a setter method that the injector uses to inject the dependency.
3. **interface injection:** the dependency provides an injector method that will inject the dependency into any client passed to it. Clients must implement an interface that exposes a setter method that accepts the dependency.

#### **So now its the dependency injection’s responsibility to:**

1. Create the objects
2. Know which classes require those objects
3. And provide them all those objects

If there is any change in objects, then DI looks into it and it should not concern the class using those objects. This way if the objects change in the future, then its DI’s responsibility to provide the appropriate objects to the class.

#### **Inversion of control —the concept behind DI**

This states that a class should not configure its dependencies statically but should be configured by some other class from outside.

It is the fifth principle of **S.O.L.I.D** — the five basic principles of object-oriented programming and design by [**Uncle Bob**](https://en.wikipedia.org/wiki/Robert\_C.\_Martin) — which states that a class should depend on abstraction and not upon concretions (in simple terms, hard-coded).

According to the principles, a class should concentrate on fulfilling its responsibilities and not on creating objects that it requires to fulfill those responsibilities. And that’s where **dependency injection** comes into play: it provides the class with the required objects.

_Note: If you want to learn about **SOLID** principles by Uncle Bob then you can head to this_ [_link_](https://scotch.io/bar-talk/s-o-l-i-d-the-first-five-principles-of-object-oriented-design#toc-single-responsibility-principle)_._
