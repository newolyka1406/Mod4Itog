<style>
    :root {
    --primary-color: rgb(251, 160, 227);
    --secodary-color: rgb(247, 109, 210);
}

* {
    box-sizing:  border-box;
}

main {
    display: flex;
    flex-wrap: wrap;
}

body{
    background-color:  var(--primary-color);
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    margin: 0;
}

header {
    padding: 10px;
    display: flex;
    justify-content: flex-end;
    background-color: var(--secodary-color);
}

.search {
    background-color: transparent;
    border: 2px solid var(--primary-color);
    border-radius: 50px;
    font-family: inherit;
    font-size: 14px;
    padding: 20px 10px;
}

.search::placeholder {
    color: wheat;
}

.search.search:focus{
    outline: none;
    background-color: #ffbacd;
}

.movie {
    width: 300px;
    margin: 10px;
    background-color: var(--secodary-color);
    box-shadow: 0 4px 5px rgba(0, 0, 0, 0.2);
    position: relative;
    overflow: hidden;
    border-radius: 3px;
}

.movie img{
    width: 100%;
}

.movie-info {
    color: black;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 20px 30px 30px;
    letter-spacing: 0.5px;
}

.movie-info h3{
    margin-top: 0;
}

.movie-info span{
    background-color: var(--primary-color);
    padding: 25px 5px;
    border-radius: 3px;
    font-weight: bold;
}

.movie-info span.green{
    color: lightgreen;
}

.overview {
    background-color: #ffbacd;
    padding: 20px;
    position: absolute;
    left: 0;
    bottom: 0;
    right: 0;
    max-width: 100%;
    transform: translateY(101%);
    transition: transform 0.3s ease-in;
}

.movie:hover .overview{
    transform: translateY(0)
}
</style>

<main id="main">
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <h3 id="MovieTitle">Летучий корабль</h3>
            <span class="black">6.9</span>
        </div>
        <div class="overview">
            <h3 id="Description">6+ ‧  ‧  ‧ Комедия/Фэнтези ‧  ‧  ‧ 1 ч 40 мин
</h3>
        </div>
    </div>
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <h3 id="MovieTitle">Кунг-Фу Панда 4</h3>
            <span class="black">9.0</span>
        </div>
        <div class="overview">
            <h3 id="Description">6+ ‧  Комедия/Приключения  1 ч 34 мин
</h3>
        </div>
    </div>
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <h3 id="MovieTitle">Лед 3</h3>
            <span class="black">9.9</span>
        </div>
        <div class="overview">
            <h3 id="Description">6+ ‧  ‧  ‧ Спорт/Романтика ‧  ‧  ‧  2 ч 14 мин
</h3>
        </div>
    </div>
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <h3 id="MovieTitle">Онегин</h3>
            <span class="black">5.8</span>
        </div>
        <div class="overview">
            <h3 id="Description">6+ ‧  ‧  ‧ Драма/Романтика ‧  ‧  ‧ 2 ч 21 мин</h3>
        </div>
    </div>
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <h3 id="MovieTitle">Ненормальный</h3>
            <span class="black">7.8</span>
        </div>
        <div class="overview">
            <h3 id="Description">12+ ‧  ‧  ‧  ‧ Комедия/Драма ‧  ‧  ‧ 1 ч 43 мин</h3>
        </div>
    </div>
    <div class="movie" id="movie">
        <div class="movie-info" id="MovieInfoDiv">
            <h3 id="MovieTitle">Водитель-олигарх</h3>
            <span class="black">?</span>
        </div>
        <div class="overview">
            <h3 id="Description">12+  ‧ Комедия
</h3>
        </div>
    </div>
</main>