# LQR & LQG Design for Control of Robotic Systems
This project aims to analyze and control a crane system that moves along a one-dimensional track. The system consists of a frictionless cart with mass 'M', actuated by an external force 'F', and two loads suspended from cables with masses 'm<sub>1</sub>' and 'm<sub>2</sub>', and lengths 'l<sub>1</sub>' and 'l<sub>2</sub>'.

## Table of Contents
1. [Introduction](#introduction)
2. [Equations of Motion](#equations-of-motion)
3. [Linearization](#linearization)
4. [Controllability](#controllability)
5. [LQR Controller](#lqr-controller)
6. [Lyapunov Stability Test](#lyapunov-stability-test)
7. [Observability](#observability)
8. [Luenberger Observer](#luenberger-observer)
9. [LQG Controller](#lqg-controller)

## Introduction
The objective of this project is to design controllers and observers for a crane system to ensure stability and optimal performance. The project is divided into two main components:
1. Derivation of equations of motion, linearization, controllability analysis, and LQR controller design.
2. Observability analysis, Luenberger observer design, LQG controller design, and system reconfiguration for reference tracking and disturbance rejection.

## Equations of Motion
We derive the equations of motion for the crane system by considering the dynamics of the cart and the suspended loads. The resulting nonlinear equations are then used to formulate the state-space representation.

## Linearization
The derived nonlinear equations are linearized around the equilibrium point to facilitate the design and analysis of the control systems. The linearized state-space representation is then used for further analysis.

## Controllability
We check the controllability of the linearized system by computing the rank of the controllability matrix. The system is controllable if the rank of the controllability matrix is equal to the number of state variables.

## LQR Controller
An LQR controller is designed to minimize a cost function that represents a trade-off between system performance and control effort. The controller optimizes the feedback gains to ensure the desired system behavior.

## Lyapunov Stability Test
The stability of the closed-loop system is analyzed using Lyapunov's indirect method by examining the eigenvalues of the closed-loop matrix. The system is stable if all eigenvalues have negative real parts.

## Observability
The observability of the system is tested by computing the rank of the observability matrix. The system is observable if the rank of the observability matrix is equal to the number of state variables.

## Luenberger Observer
A Luenberger observer is designed to estimate the unmeasurable states of the system using available input and output measurements. The observer gain matrix is determined to enhance the observability of the system.

## LQG Controller
An LQG controller, which combines the LQR and Kalman filter designs, is implemented for optimal control and state estimation in the presence of noise.

## Usage
The project files include the following MATLAB Live Scripts:
- `luenberger_observer_linear.mlx`
- `luenberger_observer_non_linear.mlx`
- `LQG_Linear.mlx`
- `LQG_nonlinear.mlx`
- `Observability.mlx`
- `LQR_Linear.mlx`
- `LQR_nonlinear.mlx`

These scripts contain the implementations for the design and analysis of the controllers and observers.

## Code Implementation and Results

<iframe width="560" height="315" src="https://www.youtube.com/watch?v=hGSncaZw_rQ&ab_channel=KoushikAlapati" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Authors
- Koushik Alapati (akoushik@terpmail.umd.edu)
- Sai Dinesh Gelam (sgelam@terpmail.umd.edu)
- Raghu Dharahas Kotla (raghu17@terpmail.umd.edu)

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments
This project is part of the ENPM667: Control of Robotic Systems course.
