Include Gardener
=================

Intorduction
-------------
This is a small C++ based commandline-tool which analyzes C/C++ code
and creates an graph or include tree.
The result can then further analyzed by other tools.

The following output formats are supported at the moment:
 - dot (Graphviz)


Build Description
-----------------

```
mkdir build
cmake ..
make
make doc
make install
```


Usage
-------
```
# analyzes recursively all files in path/to/files,
# the result is written to stdout
./include_gardener  -I path/to/files


# analyzes recursively all files in ./src and ./inc, the result is
# written to the file graph.dot
./include_gardener  -I ./src -I ./inc -o graph.dot

# the result can then be further converted to a scalable vector graphics file.
dot -Tsvg graph.dot > graph.svg

```

Contribution
------------
If you find a bug, unexpected behaviour or if you have a interesting feature
in your mind which fits to this tool, please add an issue / feature request.

Pull requests are always welcome.

License
----------

This program is free software; you can redistribute it
and/or modify it under the terms of the GNU General Public
License as published by the Free Software Foundation;
either version 3 of the License, or (at your option)
any later version.

This program is distributed in the hope that it will
be useful, but WITHOUT ANY WARRANTY; without even the
implied warranty of MERCHANTABILITY or FITNESS FOR A
PARTICULAR PURPOSE. See the GNU General Public License
for more details.

You should have received a copy of the GNU General
Public License along with this program; if not, see
<http://www.gnu.org/licenses/>.

