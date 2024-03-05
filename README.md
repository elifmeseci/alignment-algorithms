# Smith-Waterman Alignment

The Smith–Waterman algorithm performs local sequence alignment; that is, for determining similar regions between two strings of nucleic acid sequences or protein sequences. Instead of looking at the entire sequence, the Smith–Waterman algorithm compares segments of all possible lengths and optimizes the similarity measure.

<img src=https://miro.medium.com/v2/resize:fit:640/format:webp/0*1yCyyLVosToX4zNM.gif>

## Key Features
* <b>Local Alignment:</b> Unlike global alignment, the Smith-Waterman algorithm identifies the best matching part of the sequence, which is crucial for detecting functional motifs or domains in proteins or genes.
* <b>Scoring System:</b> The flexibility in scoring parameters allows for customization based on the biological context, making it adaptable to various types of sequence analysis.
* <b>Sensitivity:</b> It is highly sensitive in detecting subtle similarities, a critical feature for evolutionary studies and identifying homologous sequences.

<b>For example</b>
    <br>word1='EXTENTION'
    <br>word2='EXECUTION'
    
|   |   |   |   |   |   |   |   |   |   |
|---|---|---|---|---|---|---|---|---|---|
| E | X | - | E | C | U | T | I | O | N |
| = | = | . | = | . | . | = | = | = | = |
| E | X | T | E | - | N | T | I | O | N |

<br>MATCH = 7
<br>MISMATCH = 3





|   | 0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 |
|---|---|---|---|---|---|---|---|---|---|---|
| 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| 1 | 0 | 3 | 1 | 3 | 1 | 0 | 0 | 0 | 0 | 0 |
| 2 | 0 | 1 | 6 | 4 | 2 | 0 | 0 | 0 | 0 | 0 |
| 3 | 0 | 0 | 4 | 4 | 2 | 0 | 3 | 1 | 0 | 0 |
| 4 | 0 | 3 | 2 | 7 | 5 | 3 | 1 | 1 | 0 | 0 |
| 5 | 0 | 1 | 1 | 5 | 5 | 3 | 1 | 0 | 0 | 3 |
| 6 | 0 | 0 | 0 | 3 | 3 | 3 | 6 | 4 | 2 | 1 |
| 7 | 0 | 0 | 0 | 1 | 1 | 1 | 4 | 9 | 7 | 5 |
| 8 | 0 | 0 | 0 | 0 | 0 | 0 | 2 | 7 | 12| 10|
| 9 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 5 | 10| 15|