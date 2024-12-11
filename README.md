# Integrated Aircraft and Passenger Recovery Problem

## Project Overview

This project addresses the challenges in airline network recovery by developing a column generation post-optimization heuristic for integrated aircraft and passenger recovery. The research focuses on solving disruptions in hub-and-spoke network models while minimizing operational costs and passenger inconvenience.

## Problem Context

Commercial airlines' hub-and-spoke networks are vulnerable to various disruptions:
- Flight delays
- Reduced airport capacity
- Weather challenges
- Crew-related issues

Existing recovery methods often have limitations such as:
- Computational inefficiency
- Lack of scalability
- Inability to adapt to real-world constraints

## Implemented Approach

### Methodology
- Sequential optimization model
- Two-phase approach:
  1. Optimize aircraft rotations
  2. Assign passengers to flights

### Key Features
- Column generation heuristic
- Consideration of operational constraints
- Minimization of:
  - Downgrading costs
  - Delay costs
  - Cancellation costs

## Implementation Details

### Tools
- Optimization Solver: Gurobi
- Programming Language: Python

### Problem Formulation
- Sets:
  - Airport nodes
  - Flight legs
  - Aircraft
  - Passenger itineraries
  - Cabin classes

### Optimization Objectives
- Minimize total operational and passenger-related costs
- Ensure feasible aircraft rotations
- Maintain passenger demand satisfaction

## Experimental Results

### Test Instance Characteristics
- 85 aircraft
- 35 airports
- 608 flights
- 1,943 itineraries
- 83 flight disruptions
- 3 airport disruptions

### Key Outcomes
- Total Operating Costs: 4.21 million euros
- Delay, Downgrade, Cancellation Costs: 4.8 million dollars
- Optimal Flights Served: 291
- Passengers Transported: 28,377
- Aircraft Utilized: 78

## Potential Extensions
1. Integrate crew member scheduling
2. Develop an integrated (non-sequential) optimization approach
3. Explore machine learning methods for initial feasible solutions

## Constraints and Considerations
- Flow balance
- Demand satisfaction
- Airport capacity limitations
- Aircraft rotation feasibility

## How to Reproduce
1. Clone the repository
2. Install required dependencies
3. Configure Gurobi license
4. Run the optimization script

## Dependencies
- Gurobi Optimizer

## Future Work
- Improve computational efficiency
- Develop more robust disruption handling mechanisms
- Explore machine learning integration

## References
- Ball et al. (reference from original paper)

