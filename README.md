IMDB Movie Searching API : API interface to search and find movies by names,popularity, IMDB score directors and genres.



Setting up project and initializing data
 
virtualenv imdbEnv
source imdbEnv/bin/activate
pip install -r reuqirements.txt
python manage.py migrate
python manage.py runserver
#It populates db from imdb.json using the script populate_movies
python manage.py populate_movies

API request examples

Base API url: https://quiet-springs-15685.herokuapp.com/api/movies (For Viewing Movies)
Base API url: https://quiet-springs-15685.herokuapp.com/admin (For add/edit/remove Movies)

Filter by Name: https://quiet-springs-15685.herokuapp.com/api/movies?name=Psycho
Filter by Popularity: https://quiet-springs-15685.herokuapp.com/api/movies?popularity=83
Filter by IMDB Score: https://quiet-springs-15685.herokuapp.com/api/movies?imdb_score=8.3
Filter by Movie Name and Director: https://quiet-springs-15685.herokuapp.com/api/movies?name=Psycho&director=Alfred
Filter by Genre: https://quiet-springs-15685.herokuapp.com/api/movies?genre=horror
