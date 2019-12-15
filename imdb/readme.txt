imdb

1. Download datasets from https://datasets.imdbws.com/
2. Unzip files.
3. Import files into Mongodb


name.basics file
mongoimport --db imdb --collection name_basics --type tsv --file name.basics.tsv --fields _id,primaryName,birthYear,deathYear,primaryProfession,knownForTitles


title.ratings.tsv
mongoimport --db imdb --collection title_ratings --type tsv --file title.ratings.tsv --fields tconst,averageRating,numVotes

title.episode.tsv
mongoimport --db imdb --collection title_episode --type tsv --file title.episode.tsv --fields tconst,parentTconst,seasonNumber,episodeNumber

title.crew.tsv
mongoimport --db imdb --collection title_crew --type tsv --file title.crew.tsv --fields tconst,parentTconst,seasonNumber,episodeNumber
