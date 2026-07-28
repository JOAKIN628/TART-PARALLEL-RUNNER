# TART-PARALLEL-RUNNER
Parallel automation script for the Transient Array Radio Telescope (TART) data processing workflow.
# TART Parallel Workflow Automation

## Overview

This repository contains a parallel execution script developed as part of my undergraduate final-year project at Kenyatta University. The script automates the execution of the Transient Array Radio Telescope (TART) data processing workflow by coordinating the official TART software tools for data retrieval and processing.

The workflow was designed to reduce manual intervention, improve efficiency, and provide a reproducible approach to processing radio astronomy observations.

---

## Project Background

The Transient Array Radio Telescope (TART) is an open-source radio interferometer used for radio astronomy research. It provides software tools for retrieving and processing observational data.

As part of my final-year project, I developed a parallel execution script that automates the use of these tools. This project provides an automated workflow for processing and visualizing data from the Transient Array Radio Telescope (TART). The pipeline integrates existing TART software tools within an Apptainer container environment and automates the execution of multiple processing steps through a custom Python script.

The main script, `tart_parallel`, simplifies the TART data processing workflow by managing data acquisition, processing, image generation, background subtraction, and visualization tasks. The pipeline uses the official TART tools packaged in a container (`tart-tools.sif`) and executes them through Apptainer, ensuring a reproducible and consistent software environment.

---
## Environment Setup

The TART processing workflow uses a containerized environment to provide a consistent and reproducible software setup. The required TART software tools are obtained through a Docker image, which is converted into an Apptainer/Singularity image (`tart-tools.sif`) for execution. The container contains the necessary TART tools and dependencies required for data processing.

After preparing the container environment, the `tart_parallel` script is used to automate the processing workflow. The script runs externally and communicates with the TART tools inside the Apptainer container to perform data acquisition, processing, image generation, background subtraction, and visualization tasks. This approach ensures that the processing pipeline can be reproduced across different systems with the required container support.

---

## Features

- Automates execution of the TART data processing workflow.
- Retrieves recent and archived observational data.
- Supports parallel execution of processing tasks.
- Generates processed images from radio astronomy observations.
- Creates time-lapse videos from averaged PNG images to visualize changes across observations.
- Designed for Linux environments using Apptainer containers.
- Reduces repetitive manual commands and improves workflow reproducibility.

---

## Technologies Used

- Python
- Linux
- Apptainer
- Git
- FFmpeg
- Radio Astronomy Workflow Automation

---

## My Contribution

- Developed the parallel execution script (`./tart_parallel`).
- Automated retrieval of recent and archived TART observations.
- Integrated execution of the official TART processing tools into a single workflow.
- Generated visualization outputs, including images and videos created from averaged PNG images.
- Configured and managed the containerized execution environment.
- Tested and validated workflow execution across multiple datasets.

---

## Running the Script

```bash
./tart_parallel
```

---

## Acknowledgements

This project builds upon the official software developed by the **Transient Array Radio Telescope (TART)** project. The underlying radio astronomy processing tools were developed by the TART team. This repository contains my automation script, which orchestrates these tools to simplify and streamline the data processing workflow.

---

## Author

**Joan Akinyi**

BSc. Telecommunications and Information Technology  
Kenyatta University
