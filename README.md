# Phonetic Association Tool (Russian Version)

This application helps users memorize foreign vocabulary by connecting the sounds of new words to familiar Russian words. It uses a phonetic matching algorithm and a frequency-based dictionary to suggest the best mnemonic associations.

## Data Source & Attribution

The core dictionary used in this project (`slova.txt`) is based on high-frequency Russian vocabulary to ensure the most useful mnemonic suggestions.

*   **Source:** Data files are derived from the **University of Leeds Corpus**.
-   **Cleanup:** Corpus editing and cleanup by **William Hingston**.
-   **License:** Distributed under the **Creative Commons (CC BY) Attribution license**.

## How It Works

1.  **Input:** The user enters a foreign word phonetically (e.g., "apple" -> "эпл").
2.  **Processing:** The script normalizes the input based on Russian phonetics (handling unstressed vowels and voiced/voiceless consonant pairs).
3.  **Matching:** The tool searches the 10,000-word Leeds Corpus list using Levenshtein distance and phonetic scoring.
4.  **Story Building:** The user selects the best matches to create a memorable mental story.

## Technical Details

-   **Logic:** JavaScript-based phonetic normalization and fuzzy search.
-   **Dictionary:** 10,000 most frequent Russian words (Cyrillic only), optimized for performance.
-   **Encoding:** UTF-8.