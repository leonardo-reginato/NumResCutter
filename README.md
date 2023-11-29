# Reservoir Model Cutter 

## Description

The Reservoir Model Cutter is a tool designed to extract a specific portion of a numerical reservoir model generated by CMG software. This application enables users to create a new, smaller version of the reservoir model by providing the necessary input parameters.

## Getting Started

### Prerequisites

- Ensure you have the CMG software-generated numerical reservoir model.
- Ensure the files to be cut are saved as INCLUDE files (".inc") containing only the values of the grid property, without any keywords.
- Place the files to be cut in the same folder as the Reservoir Model Cutter files. 

### Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/your-username/reservoir-model-cutter.git
    ```

2. Install dependencies:

    ```bash
    cd reservoir-model-cutter
    pip install -r requirements.txt
    ```

## Usage

1. Run the application:

    ```bash
    python main.py --folder_dir /path/to/input --og_dimensions 46 69 30 --new_dimensions 17 10 11 --ref_corner 0 0 0
    ```

2. Follow the on-screen prompts to input the required information:

    - Select the reservoir model file.
    - Provide the model grid and its properties.
    - Define the reference cell.
    - Specify the X and Y values for the cells to cut.

3. The application will generate a new, smaller version of the reservoir model based on the provided parameters.

## Parameters

- **folder_dir**: Path to the directory containing input files.
- **og_dimensions**: Original dimensions of the reservoir model (x, y, z).
- **new_dimensions**: New dimensions for the extracted model (x, y, z).
- **ref_corner**: Reference corner coordinates for the extraction.


## Contributing

If you would like to contribute to the development of this tool, please follow our [contribution guidelines](CONTRIBUTING.md).

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgments

- The Reservoir Model Cutter is inspired by the need for a convenient tool to extract specific portions of numerical reservoir models from CMG software.
- Special thanks to the open-source community for their contributions and support.
