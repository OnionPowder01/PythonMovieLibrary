MENU_PROMPT = "\nEnter 'a' to add a movie, 'l' to see your movies, 'f' to find a movie by title, or 'q' to quit: "
movies = []


def add_movie():
    title = input("Enter the movie title: ")
    director = input("Enter the movie director: ")
    year = input("Enter the movie release year: ")

    movies.append({
        'title': title,
        'director': director,
        'year': year
    })

def show_list():
    for movie in movies:
        movie_print(movie)


def movie_print(movie):
    print(f"The title of the movie is {movie['title']}")
    print(f"The director of the movie is {movie['director']}")
    print(f"The year of release of this movie is {movie['year']}")



def find_movies():
    search_movie = input('Enter your movie title over here')

    for movie in movies:
        if movie['title'] == search_movie:
            movie_print(movie)

user_menu = {
    "a": add_movie,
    "l": show_list,
    "f": find_movies
}

def menu():
    selection = input(MENU_PROMPT)
    while selection != 'q':

        if selection in user_menu:
            variabila1 = user_menu[selection]
            variabila1()

        else:
            print('Unknown command. Please try again.')

        selection = input(MENU_PROMPT)


menu()
