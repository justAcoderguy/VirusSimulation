# Virus Spread Simulation with Matplotlib

This Python script simulates the spread of a virus using Matplotlib and is customizable for various viral parameters. The code uses a polar plot to visually represent the spread of the virus within a population.

## Overview

The code simulates the spread of a virus by modeling various aspects of the epidemic, including infections, recoveries, and deaths. It uses a polar plot to show the positions of individuals within a population and represents infected individuals with different colors.

## Features

- Customizable virus parameters, making it adaptable for different viruses.
- Visualization of the infection spread using a polar plot.
- Real-time updates of the number of infected, recovered, and deceased individuals.
- Random assignment of mild, severe, and fatal symptoms to infected individuals.

## Prerequisites

Before running the code, ensure you have the following:

- Python (3.7+)
- Matplotlib (for plotting)
- Numpy (for numerical operations)

## Customization

You can customize the virus parameters in the `COVID19_PARAMS` dictionary at the beginning of the script. Adjust the values to simulate different viruses. You can change parameters such as the basic reproduction number (r0), incubation period, recovery periods, and fatality rate.

## Function Explanations

### `class Virus`

This class represents the virus simulation. It initializes the simulation, sets up the polar plot, and contains methods for spreading the virus, updating the status, and assigning symptoms.

### `initial_population`

This method initializes the population by creating individuals and patient zero.

### `spread_virus`

This method simulates the spread of the virus. It calculates the number of new infections, handles the spread, and manages the exposed and infected individuals.

### `one_by_one`

This method is a helper for animating the spread of the virus. It adds infected individuals one by one to the plot.

### `chunks`

This method is a utility function to split a list into smaller chunks.

### `assign_symptoms`

This method assigns symptoms (mild, severe, or fatal) to infected individuals and schedules their recovery or death.

### `update_status`

This method updates the status of infected individuals, marking them as recovered or deceased.

### `update_text`

This method updates the text annotations in the plot to display current statistics.

### `gen`

A generator function that runs the simulation loop until the desired number of recoveries and deaths are achieved.

### `animate`

This method initiates the animation of the virus spread simulation.


