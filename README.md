# sqlite-practice
Containerized sqlite playground

1. Open in container with VSCode remote container extension.

2. Run the following command from inside the container (persists in host OS storage volume):
/usr/bin/sqlite3 test.db

NOTE: sqlite uses local storage and nothing more complicated than local filesystem and associated operations. The container here is really just to install the tooling to create and interact with a database that lives on our local filesystem (inefficient for other reasons, but a great setup for learning purposes)
