Nav is easy to use 3D navigation library. It operates on axis-aligned cuboids (cells). Navigation data is built on-the-fly as soon as cells are fed to the system. Separate navigation module is responsible for pathing. Exploration module can be supplied for automatic navmesh traversal. Nav was primarily created for Diablo 3 bot navigation but can be used in any project with AABB navmesh data.
For documentation check out Wiki.

Features
* dynamically builds navmesh from soup of axis-aligned cuboids
* simple navigation (set Destination, update CurrentPos, then move toward GoToPosition)
* generates exploration data allowing dynamic navmesh traversal
* simple exploration (create instance of exploration engine, update CurrentPos, then move toward GoToPosition, Destination will be automatically set by exploration engine)
* all updated and calculations are performed on separate threads, without blocking user's code execution
* automatic anti-stuck system (altering pathing when actor is potentially stuck on collision with geometry), no configuration required
* supports ray casts and ray traces
* supports both walking and flying
* NavMeshViewer allows easy viewing/debugging
