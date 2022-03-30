# open-lab-devices
Collection of repositories for various laboratory devices

The purpose of this repository to have a collection of control software written in Python and Labview for various laboratory devices. The hope is to reduce time waste when one needs a simple or more sophisticated wrapper to control equipment in the lab. 

The collection includes control software for various equipment and additional auxiliary libraries, e.g. data queues or circular buffers.

I have identified N levels of control software:
1. driver wrapper -  a collection of higher level human readable commands like:
    1. "goto", "get_Current_position" for translational stages
    2. "get_image" for a camera
2. device level - a standalone code that initializes the device and start operation
3. server level - a higher level code which allows the device code to be on the network. 
