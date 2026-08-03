# Navmeshes — off-mesh links + finer stepping + tile-seam stitch fix

On top of `navmesh_offmesh_links`, this raises Recast's tile border overlap
(TILE_BORDER_PADDING 3 -> 8) so tiles stitch across seams on continuous terrain,
closing the eroded ~1u gaps that were splitting connected ground into islands.

- Source: LandSandBoat/server branch `navmesh_offmesh_links` @ 7a8ff9cff4 + TILE_BORDER_PADDING=8
- Zones: 304
- Diff against branch `navmesh_offmesh_links` to see the stitch fix in isolation.
