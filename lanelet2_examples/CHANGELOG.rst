^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Changelog for package lanelet2_examples
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Forthcoming
-----------

1.0.0 (2020-03-03)
------------------
* Bump version to 1.0
* RoutingGraph and Route now use the new LaneletSubmap to store the lanelets they are using
  their member functions laneletMap() and passableMap() are now deprecated and should be replaced by laneletSubmap() and passableSubmap() respectively. These functions have less overhead and are less likely to be misinterpreted as 'maps containing only the lanelets you need'
* Add a new class 'LaneletSubmap' that only contains parts of the map and is faster to construct
* Routing graph and route object now support queries with a custom search function
* Improve c++17 support, supress warnings and clang-tidy 7 issues
* Simplified definition of origin in python, adapted examples
* Add examples package
* Contributors: Fabian Poggenhans, Maximilian Naumann, Sascha Wirges
