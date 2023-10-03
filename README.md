# ROS Interface Caster Generator

In the ROS2 ecosystem, C++ Functions are generally bound to Python using `pybind11`.
However, binding functions that take interfaces (`.msg` files for example) does not work.

This tool briges that gap by generating a header file providing casting capabilities between C++ to Python and back based on the works of [dimatura](https://github.com/dimatura/pyrosmsg).

The generated header can then be included in the file declaring the bindings as a normal C++ header.

Made in the context of [Heudiasyc](https://hds.utc.fr).
