# High-Level Architecture

```text
                   +----------------------+
                   |    React Frontend    |
                   +----------+-----------+
                              |
                              |
                     REST API |
                              |
                   +----------v-----------+
                   |  Node.js Backend     |
                   +----------+-----------+
                              |
              +---------------+----------------+
              |                                |
              | Redis Queue                    |
              |                                |
      +-------v--------+               +-------v-------+
      | PostgreSQL DB  |               | Python Scanner|
      +----------------+               +-------+-------+
                                              |
                                              |
                                           Tor Network
                                              |
                                              |
                                        Onion Resources
```