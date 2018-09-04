# temp_test
# test source code compiler in gcc container

# Use 1: compile and run app
 docker run --rm -v "$PWD":/usr/src/myapp -w /usr/src/myapp gcc:4.9 gcc -o myapp myapp.c

 # Use 2: run make in your container
 docker run --rm -v "$PWD":/usr/src/myapp -w /usr/src/myapp gcc:4.9 make


docker build -t my_gcc docker/.
#docker -v $(pwd):/usr/src/myapp my_gcc 
