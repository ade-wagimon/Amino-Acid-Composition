# Amino-Acid-Composition


##  This repository contains Python code for calculating residue composition of amino acid sequences.

This code provides functions to:

* Calculate the count and frequency of each amino acid residue in a given sequence.
* Handle invalid amino acid characters.
* Optionally calculate the composition of hydrophobic and hydrophilic residues based on a common hydrophobicity scale (customizable).
* Analyze a list of multiple sequences and store the results for each sequence individually.

**Getting Started:**

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/residue-composition.git
   ```
2. Install required libraries (assumes pip is installed):
   ```bash
   pip install collections
   ```

**Usage:**

1. Import the functions in your Python script:

   ```python
   from residue_composition import calculate_residue_composition, analyze_sequence_list
   ```

2. **Single Sequence Analysis:**

   ```python
   sequence = "PLEASEREPRESENTTHEINFORMATION"

   residue_composition, amino_acid_counts, hydrophobic_count, hydrophobic_freq, hydrophilic_count, hydrophilic_freq = calculate_residue_composition(sequence)

   # Access and process the results as needed
   ```

3. **Multiple Sequence Analysis:**

   ```python
   sequences = [
       "PLEASEREPRESENTTHEINFORMATION",
       "GLOBINISAFUNCTIONALPROTEIN",
   ]

   sequence_analysis = analyze_sequence_list(sequences)

   # Access results for each sequence using the sequence ID as the key in the dictionary
   ```

**Additional Notes:**

* The code defines a set of valid amino acids and a hydrophobicity scale. You can modify these based on your specific needs.
* The example usage (`main` function) demonstrates how to use the functions and print results.

I hope this README provides a clear and concise explanation of the code's functionality and usage. Feel free to leave feedback or ask questions!
