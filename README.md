The Platform Layers

This is the architecture we are going to follow throughout the entire journey.
                      Apps
                       │
        ┌──────────────┴──────────────┐
        │                             │
      REST API                       CLI
        │                             │
        └──────────────┬──────────────┘
                       │
                 Application Layer
                       │
                  Domain Layer
                       │
          Hardware Abstraction Layer
                       │
      ┌────────────────┼────────────────┐
      │                │                │
     ESP32          Gazebo Driver      PX4

The Domain owns the "what". Infrastructure owns the "how".

Model intentions, not implementations.

Every new type we introduce must answer five questions:

1-Why does this concept exist?
2-Who owns it?
3-Who depends on it?
4-Can it be replaced?
5-What invariant must always remain true?

The Domain decides what should happen. Infrastructure decides how it happens.

The owner of the abstraction is the one who needs the behavior, not the one who provides it.