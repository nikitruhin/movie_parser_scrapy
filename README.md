markdown
# 🎬 Wikipedia Movies Parser

Scrapy spider для парсинга фильмов с Wikipedia и получения рейтингов IMDb.

## 🚀 Quick Start
```bash
git clone https://github.com/nikitruhin/movie_parser_scrapy.git
cd movie_parser_scrapy
pip install scrapy requests
scrapy crawl wikipedia_movies
🔧 Features
BFS-обход категории "Фильмы по алфавиту" с кэшированием

Сбор данных: название, год, режиссер, жанр, страна

IMDb интеграция: автоматический поиск рейтинга

Очистка данных: удаление HTML/CSS/сносок [1]

Экспорт в CSV (movies.csv)

🛠 Implementation
Паук: BFS-алгоритм с контролем глубины

Pipeline:

CleanDataPipeline - очистка полей

ImdbPipeline - поиск рейтинга IMDb

Кэширование запросов для оптимизации
