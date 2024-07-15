## CourseSpeedDepth Simulator
The CourseSpeedDepth Simulator is an example program that publishes simulated data related to course, speed, and depth over Micro XRCE-DDS.

## Usage
# Running the Track Simulator
To run the CourseSpeedDepth Simulator, compile the CourseSpeedDepthPublisher.c file and execute it with the following command:

```bash
./CourseSpeedDepthPublisher <IP_address> <port> [<max_topics>]
```
Replace <IP_address> and <port> with the IP address and port number where the Micro XRCE Agent is running. <max_topics> is an optional argument specifying the maximum number of topics to publish.

# Simulator Functionality
The Simulator continuously publishes simulated data of course, speed, and depth:

```bash
Sent course: 1.0, speed: 2.8, depth: 7.2
```
Behavior
- The simulator adjusts course, speed, and depth values over time.
- Values are rounded to one decimal point and adjusted to stay within specified ranges.
- Random increments are applied to simulate dynamic changes in course, speed, and depth.

## Notes
- Ensure that the Micro XRCE Agent is running before starting the CourseSpeedDepth Simulator.
- After building the Micro XRCE Agent, you can start it with the following command:

```bash
./MicroXRCEAgent udp4 -p 8888
```

This command assumes the agent is built and installed according to the instructions provided by eProsima.

## Demo
![Simulators](https://github.com/user-attachments/assets/2d3cbd08-f54d-401d-aac1-7523d36687fb)

This GIF demonstrates the Course Simulator in action, visualizing data simulated over XRCE-DDS.

## Contact
For any questions or issues, please contact at shubhamcr10@gmail.com .
