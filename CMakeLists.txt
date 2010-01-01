project( cmodulergenerationstep )
cmake_minimum_required(VERSION 2.4)

set( CMODULER_MODULE_NAME "Example" )
set( CMODULER_MODULE_LONG_NAME "CModuler Example" )

set( CMODULER_COPYRIGHT_YEARS "2009, 2010" )

set( CMODULER_AUTHOR_NAME "Your Name Here" )
set( CMODULER_AUTHOR_EMAIL "example@example.com" )

set( CMODULER_HEADER_FILE "example.h")
set( CMODULER_HEADER_FILES_PATH_SUFFIXES "example" )

set( CMODULER_LIBRARY_NAME_RELEASE "example" )
set( CMODULER_LIBRARY_RELEASE_PATH_SUFFIXES "" )
set( CMODULER_LIBRARY_NAME_DEBUG "example exampled" )
set( CMODULER_LIBRARY_RELEASE_PATH_SUFFIXES "" )

include( ${cmodulergenerationstep_SOURCE_DIR}/CModuler )
