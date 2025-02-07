# Network Availability Script

This repository contains a Python script to calculate the yearly and seasonal availability of railroads within a municipality's domain. The output includes statistics and graphs based on the data from these railroads, helping organizations make informed decisions about their network performance.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The `network-availability` script was developed during an internship at Basler Verkehrs-Betriebe in Basel-City. It aims to provide reliable data on network availability, which can positively impact user satisfaction and contribute to well-being by enhancing autonomy, competence, and relatedness.

## Features

- Calculates network availability on a monthly and yearly basis.
- Uses shapefiles and Postgres geoinformation to analyze network data.
- Outputs results as tables, charts, and graphs.
- Supports informed decision-making based on real data.

## Installation

To use the script, you need to install the following Python libraries:

- pandas
- openpyxl
- ua_parser
- matplotlib.pyplot

You can install these libraries using pip:

```bash
pip install pandas openpyxl ua_parser matplotlib
```
