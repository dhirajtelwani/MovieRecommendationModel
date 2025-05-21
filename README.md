# Movie Recommendation System using KNN

This project builds a simple yet effective movie recommendation system using the **K-Nearest Neighbors (KNN)** algorithm. 
It recommends similar movies based on popularity, vote count, and average rating — similar to how platforms like Netflix suggest "More Like This" titles.

---

## Features

- Recommend movies based on a selected title
- Uses content-based filtering (not user-based)
- Handles duplicates (e.g., genre-exploded data)
- Includes average rating in the recommendations

---

## Tools and Technologies Used

| Tool/Library     | Purpose                                 |
|------------------|------------------------------------------|
| Python           | Core programming language                |
| Pandas           | Data manipulation and analysis           |
| Seaborn/Matplotlib | Data visualization                      |
| Scikit-learn     | Feature scaling and KNN implementation   |
| Jupyter Notebook | Interactive development and analysis     |

---

## Dataset Columns

- `Release_Year`: Year the movie was released  
- `Title`: Movie name  
- `Popularity`: Popularity score  
- `Vote_Count`: Number of votes the movie received  
- `Vote_Average`: Average user rating  
- `Genre`: Movie genre(s)  
- `Rating`: Categorized version of Vote_Average (e.g., Popular, Average)

---

## How It Works

1. The dataset is cleaned and duplicate movie entries are dropped.
2. Features like popularity, vote count, and average rating are selected.
3. These features are scaled using `StandardScaler`.
4. KNN is applied to find the top 5 similar movies for any input title.
5. The user provides a movie title, and the model prints the closest matches along with their average ratings.

---

## Why KNN?

KNN is a simple and effective choice for content-based recommendations. It works by measuring how close movies are to each other based on numerical features — making it ideal when there's no user history available.

---

## Example Output

Selected Movie: Pursuit
Vote Average: 5.9

Recommended Movies:
Restless (Rating: 5.9) : Action
Kimi (Rating: 6.3) : Thriller
Fistful of Vengeance (Rating: 5.3) : Action
Nightmare Alley (Rating: 7.1) : Crime
My Hero Academia: World Heroes' Mission (Rating: 7.3) : Animation


---

## How to Run

1. Clone this repo:
    ```
    git clone https://github.com/dhirajtelwani/MovieRecommendationModel.git
    ```

2. Install dependencies:
    ```
    pip install pandas matplotlib seaborn scikit-learn
    '''
---

## To-Do / Enhancements

- Add genre-based filtering
- Fuzzy title matching (handle typos)
- Web interface with Streamlit or Flask

---

## Author

**Dhiraj Telwani**  
  (mailto:dhirajtelwan@gmail.com) |
  [LinkedIn](https://www.linkedin.com/in/dhiraj-telwani/) | [GitHub](https://github.com/dhirajtelwani)
