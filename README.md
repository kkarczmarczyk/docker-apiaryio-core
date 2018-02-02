# docker-apiaryio-core

Newer version of apiaryio/client with --watch support.

## Usage:

### Live-preview

`docker run -v ~/path_to_apib_folder:/tmp -p 8080:8080 kkarczmarczyk/apiaryio preview --path="/tmp/api.apib" --watch --server --host=0.0.0.0`

Now, open browser at `localhost:8080`. After edit .apib, just hit F5.

### Static build

`docker run --volume ~/path_to_apib_folder:/tmp kkarczmarczyk/apiaryio preview --path="/tmp/api.apib" --output="/tmp/api.html"`