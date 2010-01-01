                                 CMODULER 1.0

INTRODUCTION

 CModuler is a CMake module generator. I was fed up with copy & paste, search
 & replace over and over again 90% of the time.

 Version 1.0 (AKA "CModuler Meta") provides only very limited functionality: it 
 will create finders (modules of the form FindXXX.cmake) for libraries.

REQUIREMENTS
 
 CModuler is nothing more than a parametrized set of CMakeLists.txt and
 templates. The only requirement is CMake itself and a text editor.

USAGE

 1. Edit CMakeLists.txt and fill in the values
 2. cd build
 3. cmake ..

 CModuler will create a 'test' directory containing the finder and a very
 simple CMakeLists.txt meant for testing. The test will be run automatically,
 if you do not want to run the test, replace step 3 with "cmake ..
 -DNO_TEST:BOOL=ON".

 The generated finder supports debug/release versions of the library, i. e:
  - if you build your application in release mode, it will be linked to the 
    release version of the third-party library.
  - if you build your application in debug mode, it will be linked to the
    debug version of the third-party library.

FUTURE
 
 I am developing a more advanced version which will allow the other 10% of
 cases: multi-library finders, search for programs, optional/mandatory tests,
 etc.

LICENSE
 
 BSD license, like CMake. See COPYING.

AUTHOR
 Pau Garcia i Quiles <pgquiles@elpauer.org>
 http://www.elpauer.org
