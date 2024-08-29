# Covert Communication via Interpacket Delays

This project demonstrates a method for covert communication by encoding a secret message within interpacket delays using a probability distribution. The goal is to minimize the chances of the secret message being intercepted by third parties by disguising the message within normal network traffic patterns.

## Project Structure

- **Proj_Files/**: This directory contains key visualizations and the secret message to be transmitted.
  - `secret_message_bits.txt`: The text file containing the bits of the secret message that need to be sent covertly.
  - `*.jpeg`: Images showcasing histograms of different interpacket delays, which are used to encode the secret message.
  
- **Data/**: Contains the baseline distribution data for interpacket delays.
  - `Traffic_data_orig.csv`: The CSV file that provides the baseline probability distribution for interpacket delays, used as a reference for encoding the message.

- `ECS256_Project_V3.ipynb`: The main Jupyter Notebook containing the code implementation. This notebook:
  - Loads the baseline distribution for interpacket delays.
  - Encodes a secret message into interpacket delays using the provided probability distribution.
  - Demonstrates the process through code and visualizations.
  - Provides analysis on the effectiveness and stealth of the covert communication.

## How It Works

1. **Baseline Distribution**: The project uses a baseline distribution of interpacket delays to mimic normal traffic patterns. This distribution is stored in `Data/baseline_distribution.csv`.

2. **Message Encoding**: The secret message, found in `Proj_Files/secret_message_bits.txt`, is encoded into a sequence of interpacket delays based on the baseline distribution. The encoding process aims to blend the delays into regular network traffic, making it difficult to detect any anomalies.

3. **Visualization**: Histograms in the `Proj_Files` directory visualize the interpacket delays. These images show the distribution of delays before and after encoding the secret message, helping to assess the stealthiness of the encoded message.

4. **Execution**: The notebook `ECS256_Project_V3.ipynb` guides you through the entire process, from loading the baseline distribution to encoding and analyzing the covert message. This includes:
   - Loading and analyzing the baseline interpacket delay distribution.
   - Encoding the secret message using the chosen distribution.
   - Visualizing the changes in interpacket delays after encoding the message.

## Usage

To run this project:
1. Clone this repository.
2. Open `ECS256_Project_V3.ipynb` in Jupyter Notebook or any compatible environment.
3. Follow the steps in the notebook to encode your secret message and analyze the results.

## Notes

- Ensure that the `Data/` and `Proj_Files/` directories are correctly populated with the necessary files before running the notebook.
- The project is designed for educational purposes to demonstrate the concept of covert communication through timing channels. It should not be used for malicious activities.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
