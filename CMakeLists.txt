# <your library name
# https://github.com/<your_user>/<repo_name>
# MIT License

cmake_minimum_required(VERSION 3.5)

idf_component_register(SRCS "hello.cpp" 
                       INCLUDE_DIRS "."
                       REQUIRES arduino)

project(<your_project>)
