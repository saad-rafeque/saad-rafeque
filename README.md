# Saad Rafique

**UAV autonomy and reinforcement learning engineer** · Islamabad, Pakistan · open to relocation (UAE, Saudi Arabia)

I build decision-making and control software for autonomous drones: multi-vehicle coordination, fault tolerance and learned obstacle avoidance on PX4 and ROS 2. Every result I report comes from logged runs measured against a stated pass limit.

### Featured projects

**[drone-swarm-failover](https://github.com/saad-rafeque/drone-swarm-failover)** · PX4, ROS 2 Jazzy, MAVROS, PPO

A 10-drone swarm that finishes its mission when the leader fails. Decentralized leader election, V-formation flight and obstacle avoidance, with no central controller.

- New leader agreed 1.4–1.7 s after the leader is killed or loses its radio; goal reached in 55 of 55 PX4 fault trials
- Exactly one leader after convergence in 1,000 of 1,000 randomized runs with crashes, delays and network splits
- Learned avoidance policy completes 71 of 90 unseen obstacle courses, against 25 of 90 for a tuned potential-field controller
- Election logic scales from 2 to 100 drones with the same takeover time
- Simulation only (PX4 SIH); flight test plan for Pixhawk 6C hardware included

**[dots-and-boxes-rl](https://github.com/saad-rafeque/dots-and-boxes-rl)** · PyTorch, Numba, MCTS

AlphaZero and a Dueling Double DQN written from scratch, with no RL library, and compared on the same board with the same input features. With tree search disabled on both sides the AlphaZero network won 200–0, while a standard benchmark bot scored the two agents within 3 points of each other. The repository documents why the benchmark failed and how the head-to-head test was built.

**[eye-gesture-control](https://github.com/saad-rafeque/eye-gesture-control)** · OpenCV, MediaPipe

Real-time gaze and blink input for hands-free cursor control. The vision front end of Sight Switch, my final-year project: smart-home control by eye movement for users with limited mobility (Raspberry Pi, MQTT, ESP32).

### Stack

| Area | Tools |
| --- | --- |
| UAV autonomy | PX4, ArduPilot, ROS 2, MAVROS, MAVLink, QGroundControl, Mission Planner, SITL |
| Learning | PyTorch, Stable-Baselines3, Gymnasium; PPO, DQN, AlphaZero / MCTS |
| Vision and embedded | OpenCV, MediaPipe, Raspberry Pi, ESP32, MQTT |
| Languages | Python, MATLAB / Simulink |
| Building next | C++ ROS 2 nodes, on-device inference on Jetson (ONNX, TensorRT) |

### Contact

saadrafiique@gmail.com · [LinkedIn](https://www.linkedin.com/in/rafeque)
