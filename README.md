![logo_transparent](https://user-images.githubusercontent.com/5942370/88551418-d623ea00-cff0-11ea-87d8-e9b94174aaa2.png)

Grav is an embedded distributed messaging library for Go applications. Grav allows interconnected components of your system to communicate effectively in a reliable, asynchronous manner. HTTP and RPC are hard to scale well in modern distributed systems, so we created Grav to add a performant and resilient messaging system to various distributed environments.

Grav's main purpose is to act as a flexible abstraction that allows your application to discover and communicate using a variety of protocols without needing to re-write any code.

Since Grav is embedded, it is instantiated as a `grav.Grav` object which your application code uses to send and recieve messages. Messages can be sent in-process (such as between Goroutines), or to other nodes via **transport plugins** such as [Websocket](./transport/websocket/README.md) and [NATS](./transport/nats/README.md). Transport plugins extend the Grav core to become a networked distributed messaging system. Grav nodes can also be configured to automatically discover each other using **discovery plugins**. Grav can operate as a decentralized mesh or integrate with centralized streaming platforms, making it extremely flexible.

## Documentation
Full documentation can be found on the [Grav docs site](https://grav.suborbital.dev).

## Project status

Grav is currently in beta, and is being developed alongside (and is designed to integrate with) [Vektor](https://github.com/suborbital/vektor) and [Reactr](https://github.com/suborbital/reactr). It is also the messaging core that powers Suborbital's flagship project, [Atmo](https://github.com/suborbital/atmo).

Copyright Suborbital contributors 2021.
