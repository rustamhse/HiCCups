# HiCCups: High-throughput Chromosome Conformation Capture Analysis Tool

## Introduction

HiCCups is a PyQt5-based desktop application designed for processing High-throughput Chromosome Conformation Capture (Hi-C) data. Starting from raw FASTQ files, our tool provides an end-to-end solution, including read alignment, Hi-C data processing, and visualization of chromosomal interactions through heatmaps. 

## Features

- **Iterative Read Alignment**: Utilizes Bowtie2 for efficient and accurate mapping of Hi-C sequencing reads.
- **Genomic Data Processing**: Parses aligned data to construct structured Hi-C fragments, applying filters to remove duplicates and aberrant large fragments.
- **Heatmap Generation**: Produces high-resolution heatmaps representing chromosomal interactions, showcasing data after iterative correction processes.
- **Interactive Interface**: Includes tabs for setting input parameters, monitoring progress through a console output, and visualizing results in a heatmap format.

## System Requirements

- **Operating System**: Windows, Linux, or macOS
- **Python Version**: Python 3.6 or higher
- **Dependencies**:
  - PyQt5
  - matplotlib
  - numpy
  - hiclib
  - mirnylib
  - samtools

## Installation

To set up HiCCups, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/hiccups.git
   ```
2. Install the required Python packages:
   ```bash
   pip install PyQt5 matplotlib numpy
   ```
3. Ensure Bowtie2 and other required tools are installed and correctly configured in your system.

## Usage

To run HiCCups, navigate to the directory containing the tool and execute:

```bash
python main.py
```

Follow the on-screen instructions to input the necessary files and parameters:

- **Bowtie2 Directory Path**
- **Genome File** (.fa format, including chromosome and enzyme information)
- **FASTQ Files** for the left and right sides of the DNA molecule

After configuring the inputs, proceed with the analysis by clicking the 'Proceed' button. Monitor the progress in the 'Console Output' tab and view the generated heatmap under the 'Heatmap' tab.

## Output

The main outputs of HiCCups include:

- **HDF5 File**: Contains the Hi-C heatmap data, illustrating the strength of chromosomal interactions.
- **PDF File**: A visual representation of the heatmap for easier interpretation and analysis.

## Contributing

Contributions to HiCCups are welcome. Please fork the repository and submit pull requests with your enhancements. For major changes, please open an issue first to discuss what you would like to change.

## License

Distributed under the MIT License. See `LICENSE` for more information.

## Contact

Rustam Ziyoev - [ziyoevr@yandex.ru](mailto:ziyoevr@yandex.ru)

Project Link: [https://github.com/yourusername/hiccups](https://github.com/yourusername/hiccups)
