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