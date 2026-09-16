### Plygon

Technical artist. Procedural systems, DCC tooling, and cross-application pipelines.

HOWEST DAE, Game Graphics Production. Working stack: Blender (`bpy`, Geometry Nodes, shader / compositor graphs), Houdini (SOP, VEX, HDAs), Python, Unreal Engine PCG.

**[Plygon MCP](https://github.com/Plygonality/Plygon-mcp)** | flagship  
Local FastMCP bridges for controlling DCC applications through a consistent tool interface. A DCC-side TCP listener executes commands on the main thread, supporting scene inspection, mutation, viewport capture, and export.

| DCC | Bind | Process |
|---|---|---|
| Blender 3.0+ | `127.0.0.1:9876` | add-on + `plygon-blender-mcp` |
| Houdini 19.5+ | `127.0.0.1:9877` | package + `plygon-houdini-mcp` |

MIT licensed. Localhost only. No telemetry.

**[NodeBridge](https://github.com/Plygonality/NodeBridge)** | flagship  
Cross-DCC translation layer for procedural node systems. Converts Blender Geometry Nodes, Shader Nodes, and Compositor graphs into a structured intermediate representation that can be reconstructed as native systems in other DCCs, including Houdini and Unreal Engine.

The goal is not to copy node layouts literally. NodeBridge translates the underlying procedural logic, parameters, connections, and data flow into equivalent structures for the target application.

Together, **Plygon MCP** and **NodeBridge** form the core tooling layer: one provides programmatic access to DCC applications, the other makes procedural systems portable between them.

**[gn-as-code](https://github.com/Plygonality/gn-as-code)**  
Python API for building, dumping, and diffing Blender Geometry Node trees as data. Git is the source of truth; the `.blend` file is a working cache. Graphs can be reconstructed, compared structurally, and applied through Plygon MCP.

**[HDA-as-code](https://github.com/Plygonality/HDA-as-code)**  
Houdini counterpart to gn-as-code. Typed SOP network builders, canonical graph representation, and structural diffs for procedural Houdini systems. The `.hip` file becomes a working cache rather than the only source of truth.

**[Master Node](https://github.com/Plygonality/Master-Node)**  
Blender N-panel framework for exposing parameters from category-level master node groups. Designed for procedural material systems where individual materials are parameter configurations rather than independent node trees.

**[Hard Sci-Fi Idea Generator](https://github.com/Plygonality/Hard-SciFi-idea-generator)**  
Hard sci-fi concept generator for 3D artists. Produces structured megastructure and environment concepts with physical constraints, lighting, palette, scale, and composition guidance.

The repositories share the same direction: procedural graphs as data, portable systems instead of isolated files, and tools that reduce repetitive DCC work.

[ArtStation](https://www.artstation.com/emil_van_dam) · [LinkedIn](https://www.linkedin.com/in/emil-van-dam-220731198) · [YouTube](https://youtube.com/@emiiiill20)