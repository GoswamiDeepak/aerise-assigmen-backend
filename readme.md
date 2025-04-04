# Sequence Diagram
```text
+---------+       +------------+       +-----------+
| Vehicle |       | Node.js API|       | React App |
+---------+       +------------+       +-----------+
     |                   |                   |
     |  Send Event Data  |                   |
     |------------------>|                   |
     |                   |                   |
     |                   |  HTTP Request     |
     |                   |<------------------|
     |                   |                   |
     |                   |  JSON Response    |
     |                   |------------------>|
     |                   |                   |
```

# Use Case Diagram
```text
+----------------+
| Vehicle System |
+----------------+
       |
       | Generates
       v
+----------------+     +-------------------+     +-----------------+
| Ignition Events|     | Time Interval Data|     | Health Metrics  |
+----------------+     +-------------------+     +-----------------+
       |                       |                       |
       v                       v                       v
+----------------------------------------------------+
|                 Node.js Proxy Server                |
+----------------------------------------------------+
       |
       | Provides data to
       v
+----------------------------------------------------+
|                 React Web Portal                   |
+----------------------------------------------------+
       |                   |                   |
       v                   v                   v
+------------+     +----------------+     +-----------+
| View Events|     | Filter/Search  |     | Dashboard |
+------------+     +----------------+     +-----------+
```