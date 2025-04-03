# MuseFlow: A Keyword-Controlled Music Generation System

MuseFlow is an AI system that helps musicians overcome creative blocks by generating musical flows based on user-supplied keywords. The system converts descriptive keywords into detailed text prompts using a custom mapping layer and then utilizes the pre-trained MusicGen model to generate music. This project is designed to run in Google Colab and features an interactive UI built with ipywidgets.

## Features

- **Keyword-to-Music Mapping:**  
  MuseFlow converts user keywords (e.g., "rock", "love", "mysterious") into detailed text prompts that incorporate musical parameters such as tempo, instrumentation, harmony, dynamics, rhythm complexity, mood intensity, and genre influence.

- **Interactive Control:**  
  The interactive UI allows users to:
  - Enter keywords.
  - Select additional descriptive adjectives.
  - Adjust extra parameters (energy, rhythm complexity, mood intensity, and genre influence).
  - Set the desired music duration (from 1 to 60 seconds).
  - Choose the number of outputs to generate.
  - View progress via a progress bar during music generation.

- **Multiple Output Generation:**  
  MuseFlow can generate multiple music samples for a given prompt, allowing users to compare outputs and select their favorite.

## Setup Instructions

### Running in Google Colab

1. **Open the Notebook:**
   - Download the project files and open the Colab notebook named `MuseFlow.ipynb`.

2. **Install Dependencies:**
   - In the first cell, install the required packages by running:
     ```bash
     !pip install "numpy<2"
     !pip install huggingface_hub audiocraft
     ```
   - This project is optimized to run in Google Colab.

3. **Run All Cells Sequentially:**
   - Follow the instructions in the notebook cells to set up the mapping layer, load the MusicGen model, and interact with the UI.

## Usage

1. **Input a Keyword:**
   - Enter a keyword (e.g., "rock", "love", "mysterious") in the provided text box.
2. **Refresh Descriptors:**
   - Click the "Refresh Descriptors" button to update additional descriptive options based on the keyword.
3. **Adjust Parameters:**
   - Use the dropdowns and text fields to adjust energy, rhythm complexity, mood intensity, and genre influence.
   - Set the desired music duration (using the slider from 1 to 60 seconds).
   - Choose the number of outputs to generate.
4. **Generate Music:**
   - Click the "Generate Music" button. A progress bar will indicate the generation process, and audio players will appear for each generated output.
5. **Evaluate Outputs:**
   - Listen to the generated music samples and compare them.

## Project Structure

## Development Process Documentation

During the development of MuseFlow, the following process was followed:

- **Initial Proposal & Concept Design:**
  - Defined the project concept: converting descriptive keywords into musical parameters and generating music using a pre-trained model.
  - Designed a mapping layer to translate keywords into parameters such as tempo, instrumentation, and mood.
  
- **Prototype Development:**
  - Developed a basic Colab notebook that integrated a pre-trained MusicGen model.
  - Created an interactive UI using ipywidgets to allow real-time user control over various parameters.
  - Implemented multiple output generation and progress feedback for improved user experience.
  
- **Iterative Refinement:**
  - Expanded the mapping dictionary to cover multiple popular genres.
  - Added error handling to manage out-of-range inputs and refined the UI layout using HBox and VBox.
  - Introduced additional controls for duration and extended parameters (energy, rhythm complexity, mood intensity, genre influence).
  
- **Testing and Debugging:**
  - Performed extensive testing in Google Colab to ensure smooth integration and performance.
  - Documented each step of the development process and maintained version control using Git.
  
- **Finalization:**
  - Consolidated the code, created the README, and prepared sample outputs for submission.
  - Generated a demo video documenting system functionality for inclusion in the final presentation.

## Notes


  - **Environment:**  
  MuseFlow is designed to run in Google Colab. Local setup may require additional configuration (e.g., GPU support).

- **Future Enhancements:**  
  Future work could include expanding the parameter set, refining the interactive UI, and integrating a richer user feedback mechanism.

## License

This project is licensed under the SFU License.


