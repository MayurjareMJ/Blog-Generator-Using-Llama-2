# Blog Generator Using LLaMA 2 with Streamlit

This project is a web application that generates blogs based on user inputs using the LLaMA 2 language model. The app allows users to specify the topic, word limit, and target audience to create custom blogs with ease.

## Features
- User-friendly interface built with Streamlit.
- Supports generating blogs for different writing styles (e.g., researchers, data scientists, common people).
- Utilizes the LLaMA 2 model for generating high-quality text.

## Requirements

To run this project locally, you'll need the following:

- Python 3.8 or higher
- Streamlit
- LangChain
- CTransformers
- LLaMA 2 model file (`llama-2-7b-chat.ggmlv3.q6_K.bin`)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/blog-generator-llama2.git
   cd blog-generator-llama2
   ```

2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install the required Python packages:
   ```bash
   pip install -r requirements.txt
   ```

4. Place the LLaMA 2 model file (`llama-2-7b-chat.ggmlv3.q6_K.bin`) in the `models` directory.

## Usage

1. Run the Streamlit app:
   ```bash
   streamlit run app.py
   ```

2. Open your browser and navigate to the URL displayed in the terminal (typically `http://localhost:8501`).

3. Enter the blog topic, specify the word limit, and select the target audience. Click the "Generate" button to get the blog content.

## File Structure

```
.
├── app.py                   # Main application script
├── models
│   └── llama-2-7b-chat.ggmlv3.q6_K.bin  # LLaMA 2 model file
├── requirements.txt         # List of required Python packages
└── README.md                # Project documentation
```

## Requirements File

Add the following dependencies to your `requirements.txt`:

```
streamlit
langchain
ctransformers
```

## Notes

- Ensure that the LLaMA 2 model file is downloaded and placed in the `models` directory before running the app.
- Adjust the configuration of the `CTransformers` object in `app.py` as needed to fit your system's capabilities.

## Contributing

Contributions are welcome! Feel free to fork this repository and submit a pull request with your changes.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

## Acknowledgements

- [LLaMA 2 by Meta](https://ai.meta.com/llama/) for the powerful language model.
- [Streamlit](https://streamlit.io/) for the user-friendly web app framework.
- [LangChain](https://langchain.com/) for prompt handling.
