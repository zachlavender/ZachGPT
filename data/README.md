# Training Data

This directory contains the training data for ZachGPT.

## Directory Structure

- `raw/` - Original text datasets (not tracked in git)
- `processed/` - Tokenized and preprocessed data (not tracked in git)

## Data Sources

Add information about your training data sources here:

### Suggested Datasets for Educational Purposes

1. **Tiny Shakespeare**
   - Source: https://raw.githubusercontent.com/karpathy/char-rnn/master/data/tinyshakespeare/input.txt
   - Size: ~1MB
   - Good for: Initial testing and quick iterations
   - License: Public domain

2. **OpenWebText** (subset)
   - Source: https://github.com/jcpeterson/openwebtext
   - Size: Configurable
   - Good for: More diverse training data
   - License: Various (check individual sources)

3. **Project Gutenberg**
   - Source: https://www.gutenberg.org/
   - Size: Variable
   - Good for: Literary text, public domain books
   - License: Public domain

4. **Wikipedia** (subset)
   - Source: https://dumps.wikimedia.org/
   - Size: Configurable
   - Good for: Factual, encyclopedic text
   - License: Creative Commons

## Adding New Data

To add a new dataset:

1. Download the raw data to `data/raw/`
2. Create a preprocessing script in `Python/` (to be implemented)
3. Process the data and save to `data/processed/`
4. Update this README with dataset information

## Data Format

### Raw Data
- Text files (.txt)
- One document per file or large corpus files
- UTF-8 encoding

### Processed Data
- NumPy arrays (.npy, .npz)
- Tokenized sequences
- Vocabulary files

## Notes

- Data files are gitignored to keep repository size manageable
- Always document data sources and licenses
- Keep sample datasets small for quick experimentation
- For production training, use larger, more diverse datasets
