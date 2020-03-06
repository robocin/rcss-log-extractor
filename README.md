# RcssLogExtractor 
The RcssLogExtractor is a tool developed to help RoboCup Simulation Soccer 2D developers, giving a better format file of the rcssserver logs where it can be made game analyzes. This extractor gets `.rcg` files and transform to `.csv` files with all informations of the simulation 2d games, provides by the rcssserver. All features extracted are listed here:

* **Cycles**: The game cycles.
* **Play Mode**: The play mode per cycle.
* **Teams Score**: The left and right score per cycle.
* **Position**: The x and y position of the ball and each player per cycle.
* **Velocity**: The velocity on axis x and y of the ball and each player per cycle.
* **Players Body Angle**: The body angle of each player per cycle.
* **Players Neck Angle**: The neck angle of each player per cycle.
* **Players Point To**: The point to axis x and y of each player per cycle.
* **Players View**: The view quality and view width of each player per cycle.
* **Players Attribute**: The stamina, effort, recovery and stamina capacity of each player per cycle.
* **Players Focus**: The focus side and unum of each player per cycle.
* **Players Counting**: The counting kick, dash, turn, catch, move, turn neck, change view, say, tackle, point to and attention to of each player per cycle.


## Installation

To install the requires libraries run:

    $ sudo apt-get install default-jre default-jdk

## How to use

```sh
cd bin/
./rcssLogExtractor --in "path-to-folder-with-logs-in-rcg" --out "path-to-folder-to-put-csv-files"
```

Obs: the usage of `" "` to path arguments is optional on ubuntu. To more options, use `./rcssLogExtractor --help`.