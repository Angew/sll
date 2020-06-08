# Copyright Petr Kmoch 2020
# Distributed under the Boost Software License, Version 1.0
# (See accompanying LICENSE.txt or copy at https://www.boost.org/LICENSE_1_0.txt)

cmake_minimum_required(VERSION 3.14)
project(SllProject)

add_subdirectory(library)

option(
	SLL_BUILD_PLAYGROUND
	"Include the Playground project in the generated buildsystem"
)
if(SLL_BUILD_PLAYGROUND)
	add_subdirectory(playground)
endif()
