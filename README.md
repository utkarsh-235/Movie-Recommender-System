---
# Movie Recommender System

A Python-based Movie Recommender System that suggests movies to users based on their input. This project leverages libraries like `sklearn`, `numpy`, `pandas`, and `difflib` to create an efficient and easy-to-use recommendation engine.

---

## Features

- **Content-based filtering:** Recommends movies based on similarities between their features (e.g., genre, actors, director, etc.).
- **Dynamic search:** Uses the `difflib` library to suggest movies even if the input name is partially or incorrectly spelled.
- **Simple and interactive interface:** Users can input a movie title and get a list of similar movies.

---

## Libraries Used

- **Python:** Core programming language for the project.
- **pandas:** For handling and analyzing structured data.
- **numpy:** For numerical operations and data manipulation.
- **sklearn (scikit-learn):** For computing cosine similarity between movie feature vectors.
- **difflib:** To provide approximate string matching for handling typos and variations in movie titles.

---

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/movie-recommender.git
   cd movie-recommender
   ```

2. Install the required Python packages:
   ```bash
   pip install pandas numpy scikit-learn
   ```

---

## Dataset

The system uses a **movies dataset** containing information such as:

- Movie title
- Genre
- Director
- Cast
- Keywords

You can use popular datasets like [TMDB 5000 Movie Dataset](https://www.kaggle.com/tmdb/tmdb-movie-metadata) or any other similar data source.

---

## How It Works

1. The data is preprocessed to create feature vectors based on relevant attributes such as genre, cast, and director.
2. Cosine similarity is calculated between the feature vectors of all movies.
3. When a user inputs a movie title, the system:
   - Matches the title to the closest valid one using `difflib.get_close_matches`.
   - Finds movies with the highest cosine similarity scores.
4. The top recommendations are displayed as output.

---

## Usage

Run the program with:
```bash
python movie_recommender.py
```

Then, follow the prompts to input a movie title and view the recommendations.

---

## Example Output

**Input:**  
`"Avangers"` (intentionally misspelled)

**Output:**  
```
Did you mean: "Avengers: Infinity War"?

Top 5 Recommendations:
1. Avengers: Endgame
2. Guardians of the Galaxy
3. Iron Man 3
4. Thor: Ragnarok
5. Captain America: Civil War
```

---

## Contributing

Contributions are welcome! Feel free to submit a pull request or report issues to improve this project.

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

---

## Author

**Utkarsh**  
LinkedIn: [Utkarsh Agarwal](https://www.linkedin.com/in/utkarsh-agarwal-a0811a263)

--- 

Let me know if you'd like any modifications or additional sections!
