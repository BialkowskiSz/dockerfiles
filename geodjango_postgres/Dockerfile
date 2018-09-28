#   Run postgres with geospatial libraries (postgis)
#
#   docker run -d \
#              --name geo_postgres \
#              -p 5432:5432 \
#              -e POSTGRES_PASSWORD=admin \
#              bialkowskisz/geodjango_postgres

FROM postgres:10.5

LABEL maintainer "Szymon Bialkowski bialkowski.sz@gmail.com"

RUN apt-get update && \
    apt-get install -y \
    postgresql postgresql-contrib \
    postgis \
    binutils libproj-dev gdal-bin
