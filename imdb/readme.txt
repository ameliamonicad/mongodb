imdb

1. Download datasets from https://datasets.imdbws.com/
2. Unzip files.
3. Import files into Mongodb


name.basics file

mongoimport --db imdb --collection name_basics --type tsv --file name.basics.tsv --fields _id,primaryName,birthYear,deathYear,primaryProfession,knownForTitles
