# VS Code Setup for ROS2 Node Debugging

## How to debug binary files
This option is suitable for debugging programs that are started by executing the binary file directly.

1. Open the launch.json and in the launch configuration "Debug Catch2 tests" set the variable "program" to the absolute path of the binary file.
2. Go to the Debug Console in VS Code. In the drop-down menu next to the "Start Debugging" icon select the configuration "Debug Catch2 tests".
3. Press F5 to start debugging.


## How to debug a running process
This options is suitable for debugging a ROS 2 node that is started with a launch file.

1. Open the launch.json and in the launch configuration "Attach to ROS 2 Node" set the variable "program" to the absolute path of the binary file of the node.
2. Go to the Debug Console in VS Code. In the drop-down menu next to the "Start Debugging" icon select the configuration "Attach to ROS 2 Node".
3. Start the node with the launch file.
4. Press F5 to start debugging.
5. When VS Code requests the process to attach to, search for the name of the binary file from step 1.
6. You have to allow the debugger to connect to the running process and have to enter the sudo password in the terminal when requested.

