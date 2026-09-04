# IMDB Movies — SQL Queries with Results

13 real business questions, answered one query at a time — from a single `SELECT *` to multi-table joins.

**Database:** `project_movie_database`
**Tables:** `movies`, `directors`
**SQL skills covered:** filtering · sorting · aggregating · joining

---

## Database Schema

Two related tables, linked by a foreign key.

**`movies`**
| Column | Description |
|---|---|
| `id` | Unique movie identifier |
| `original_title` | The film's title |
| `popularity` | IMDB popularity score |
| `revenue` | Box-office revenue |
| `vote_average` | Average audience rating |
| `release_date` | Theatrical release date |
| `director_id` | Links to `directors.id` |

**`directors`**
| Column | Description |
|---|---|
| `id` | Unique director identifier |
| `name` | Director's full name |
| `gender` | Coded gender (1 = female) |

**Relationship:** `movies.director_id → directors.id`

## Queries & Results

### Basic Retrieval
| # | Question | Result |
|---|---|---|
| A | Get all movie data | 47 rows × 13 columns |
| B | Get all director data | 1,000 rows × 5 columns |
| C | Count total movies | 47 movies |

### Filtering & Search
| # | Question | Result |
|---|---|---|
| D | Find specific directors (James Cameron, Luc Besson, John Woo) | 3 directors found |
| E | Directors whose name starts with "S" | 174 directors found |
| F | Count female directors | 150 out of 1,000 |
| G | The 10th female director (by id order) | Angelina Jolie |

### Ranking & Top-N
| # | Question | Result |
|---|---|---|
| H | 3 most popular movies | Jurassic World (418), Captain America: Civil War (198), Avatar (150) |
| I | 3 most bankable movies (by revenue) | Avatar ($2.79B), Titanic ($1.85B), The Avengers ($1.52B) |
| J | Best-rated movie since 2000 | The Dark Knight Rises — 7.6 (tied with 2 others) |

### Joins & Relationships
| # | Question | Result |
|---|---|---|
| K | Movies directed by Brenda Chapman | 0 rows — no matches in this 47-movie sample |
| L | Director with the most movies | Gore Verbinski — 3 movies (tied with 2 others) |
| M | Most bankable director (by total revenue) | James Cameron — $4.63B total revenue |

## SQL Toolkit Recap

| Concept | Purpose | Used in |
|---|---|---|
| `SELECT` / `FROM` | Retrieve columns from a table | A, B |
| `WHERE` | Filter rows by a condition | D, F, J |
| `LIKE '%'` | Pattern-match text values | E |
| `COUNT` / `SUM` | Aggregate many rows into one number | C, F, L, M |
| `GROUP BY` | Bucket rows before aggregating | L, M |
| `ORDER BY` | Sort results ascending or descending | H, I, J |
| `LIMIT` / `OFFSET` | Cap results or page through them | G, H, I |
| `JOIN ... ON` | Combine two related tables | K, L, M |

## Repository Contents

| File | Description |
|---|---|
| `IMDB_Movies_SQL_Queries_with_Results.pptx` | 16-slide deck walking through all 13 queries with syntax breakdowns and results |
